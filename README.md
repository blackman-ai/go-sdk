# Blackman AI Go SDK

Official Go client for [Blackman AI](https://www.useblackman.ai) - The AI API proxy that optimizes token usage to reduce costs.

## Features

- 🚀 Drop-in replacement for OpenAI, Anthropic, and other LLM APIs
- 💰 Automatic token optimization (save 20-40% on costs)
- 📊 Built-in analytics and cost tracking
- 🔒 Enterprise-grade security with SSO support
- ⚡ Low latency overhead (<50ms)
- 🎯 Semantic caching for repeated queries

## Installation

```bash
go get github.com/blackman-ai/go-sdk
```

## Quick Start

```go
package main

import (
    "context"
    "fmt"
    "log"

    blackman "github.com/blackman-ai/go-sdk"
)

func main() {
    // Configure client
    cfg := blackman.NewConfiguration()
    cfg.Host = "app.useblackman.ai"
    cfg.Scheme = "https"
    cfg.AddDefaultHeader("Authorization", "Bearer sk_your_blackman_api_key")

    client := blackman.NewAPIClient(cfg)
    ctx := context.Background()

    // Create completion request
    req := blackman.CompletionRequest{
        Provider: "OpenAI",
        Model:    "gpt-4o",
        Messages: []blackman.Message{
            {
                Role:    "user",
                Content: "Explain quantum computing in simple terms",
            },
        },
    }

    // Send request
    resp, _, err := client.CompletionsAPI.Completions(ctx).CompletionRequest(req).Execute()
    if err != nil {
        log.Fatal(err)
    }

    fmt.Println(resp.Choices[0].Message.Content)
    fmt.Printf("Tokens used: %d\n", resp.Usage.TotalTokens)
}
```

## Authentication

Get your API key from the [Blackman AI Dashboard](https://app.useblackman.ai/settings/api-keys).

```go
cfg := blackman.NewConfiguration()
cfg.Host = "app.useblackman.ai"
cfg.Scheme = "https"
cfg.AddDefaultHeader("Authorization", "Bearer sk_your_blackman_api_key")
```

## Context and Cancellation

All API calls accept a `context.Context` for cancellation and timeouts:

```go
ctx, cancel := context.WithTimeout(context.Background(), 30*time.Second)
defer cancel()

resp, _, err := client.CompletionsAPI.Completions(ctx).CompletionRequest(req).Execute()
if err != nil {
    if ctx.Err() == context.DeadlineExceeded {
        log.Println("Request timeout")
    }
    log.Fatal(err)
}
```

## Framework Integration

### Gin Web Framework

```go
package main

import (
    "context"
    "net/http"

    "github.com/gin-gonic/gin"
    blackman "github.com/blackman-ai/go-sdk"
)

func main() {
    r := gin.Default()

    // Initialize Blackman client
    cfg := blackman.NewConfiguration()
    cfg.Host = "app.useblackman.ai"
    cfg.Scheme = "https"
    cfg.AddDefaultHeader("Authorization", "Bearer "+os.Getenv("BLACKMAN_API_KEY"))

    client := blackman.NewAPIClient(cfg)

    r.POST("/chat", func(c *gin.Context) {
        var input struct {
            Message string `json:"message"`
        }

        if err := c.BindJSON(&input); err != nil {
            c.JSON(http.StatusBadRequest, gin.H{"error": err.Error()})
            return
        }

        req := blackman.CompletionRequest{
            Provider: "OpenAI",
            Model:    "gpt-4o",
            Messages: []blackman.Message{
                {Role: "user", Content: input.Message},
            },
        }

        resp, _, err := client.CompletionsAPI.Completions(c.Request.Context()).
            CompletionRequest(req).Execute()
        if err != nil {
            c.JSON(http.StatusInternalServerError, gin.H{"error": err.Error()})
            return
        }

        c.JSON(http.StatusOK, resp)
    })

    r.Run(":8080")
}
```

### Echo Framework

```go
package main

import (
    "net/http"
    "os"

    "github.com/labstack/echo/v4"
    blackman "github.com/blackman-ai/go-sdk"
)

func main() {
    e := echo.New()

    // Initialize client
    cfg := blackman.NewConfiguration()
    cfg.Host = "app.useblackman.ai"
    cfg.Scheme = "https"
    cfg.AddDefaultHeader("Authorization", "Bearer "+os.Getenv("BLACKMAN_API_KEY"))

    client := blackman.NewAPIClient(cfg)

    e.POST("/chat", func(c echo.Context) error {
        var input struct {
            Message string `json:"message"`
        }

        if err := c.Bind(&input); err != nil {
            return c.JSON(http.StatusBadRequest, map[string]string{"error": err.Error()})
        }

        req := blackman.CompletionRequest{
            Provider: "OpenAI",
            Model:    "gpt-4o",
            Messages: []blackman.Message{
                {Role: "user", Content: input.Message},
            },
        }

        resp, _, err := client.CompletionsAPI.Completions(c.Request().Context()).
            CompletionRequest(req).Execute()
        if err != nil {
            return c.JSON(http.StatusInternalServerError, map[string]string{"error": err.Error()})
        }

        return c.JSON(http.StatusOK, resp)
    })

    e.Start(":8080")
}
```

## Advanced Usage

### Custom HTTP Client

```go
import (
    "net/http"
    "time"
)

cfg := blackman.NewConfiguration()
cfg.HTTPClient = &http.Client{
    Timeout: 60 * time.Second,
    Transport: &http.Transport{
        MaxIdleConns:        100,
        MaxIdleConnsPerHost: 10,
    },
}

client := blackman.NewAPIClient(cfg)
```

### Error Handling

```go
resp, httpResp, err := client.CompletionsAPI.Completions(ctx).
    CompletionRequest(req).Execute()

if err != nil {
    // Check for API error
    if apiErr, ok := err.(blackman.GenericOpenAPIError); ok {
        fmt.Printf("API Error: %s\n", apiErr.Error())
        fmt.Printf("Response Body: %s\n", apiErr.Body())
    }

    // Check HTTP status
    if httpResp != nil {
        fmt.Printf("HTTP Status: %d\n", httpResp.StatusCode)
    }

    log.Fatal(err)
}
```

### Retry Logic

```go
import (
    "github.com/cenkalti/backoff/v4"
)

operation := func() error {
    resp, _, err := client.CompletionsAPI.Completions(ctx).
        CompletionRequest(req).Execute()
    if err != nil {
        return err
    }

    // Process response
    fmt.Println(resp.Choices[0].Message.Content)
    return nil
}

err := backoff.Retry(operation, backoff.NewExponentialBackOff())
if err != nil {
    log.Fatal(err)
}
```

## Documentation

- [Full API Reference](https://app.useblackman.ai/docs)
- [Getting Started Guide](https://app.useblackman.ai/docs/getting-started)
- [Go Examples](https://github.com/blackman-ai/go-sdk/tree/main/examples)
- [GoDoc](https://pkg.go.dev/github.com/blackman-ai/go-sdk)

## Requirements

- Go 1.21 or higher
- `golang.org/x/oauth2` for authentication

## Support

- 📧 Email: [support@blackman.ai](mailto:support@blackman.ai)
- 💬 Discord: [Join our community](https://discord.gg/blackman-ai)
- 🐛 Issues: [GitHub Issues](https://github.com/blackman-ai/go-sdk/issues)

## License

MIT © Blackman AI
