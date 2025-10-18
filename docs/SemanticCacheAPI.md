# \SemanticCacheAPI

All URIs are relative to *https://app.useblackman.ai/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetConfig**](SemanticCacheAPI.md#GetConfig) | **Get** /v1/semantic-cache/config | Get semantic cache configuration for the current account
[**GetStats**](SemanticCacheAPI.md#GetStats) | **Get** /v1/semantic-cache/stats | Get semantic cache statistics including hit rate and savings
[**InvalidateAll**](SemanticCacheAPI.md#InvalidateAll) | **Delete** /v1/semantic-cache/invalidate | Invalidate all cache entries for the current account
[**UpdateConfig**](SemanticCacheAPI.md#UpdateConfig) | **Put** /v1/semantic-cache/config | Update semantic cache configuration for the current account



## GetConfig

> SemanticCacheConfig GetConfig(ctx).Execute()

Get semantic cache configuration for the current account

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SemanticCacheAPI.GetConfig(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SemanticCacheAPI.GetConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetConfig`: SemanticCacheConfig
	fmt.Fprintf(os.Stdout, "Response from `SemanticCacheAPI.GetConfig`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetConfigRequest struct via the builder pattern


### Return type

[**SemanticCacheConfig**](SemanticCacheConfig.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetStats

> SemanticCacheStats GetStats(ctx).Execute()

Get semantic cache statistics including hit rate and savings

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SemanticCacheAPI.GetStats(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SemanticCacheAPI.GetStats``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetStats`: SemanticCacheStats
	fmt.Fprintf(os.Stdout, "Response from `SemanticCacheAPI.GetStats`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetStatsRequest struct via the builder pattern


### Return type

[**SemanticCacheStats**](SemanticCacheStats.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## InvalidateAll

> InvalidateResponse InvalidateAll(ctx).Execute()

Invalidate all cache entries for the current account

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SemanticCacheAPI.InvalidateAll(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SemanticCacheAPI.InvalidateAll``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `InvalidateAll`: InvalidateResponse
	fmt.Fprintf(os.Stdout, "Response from `SemanticCacheAPI.InvalidateAll`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiInvalidateAllRequest struct via the builder pattern


### Return type

[**InvalidateResponse**](InvalidateResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateConfig

> UpdateConfig(ctx).SemanticCacheConfig(semanticCacheConfig).Execute()

Update semantic cache configuration for the current account

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	semanticCacheConfig := *openapiclient.NewSemanticCacheConfig(false, float64(123), int64(123)) // SemanticCacheConfig | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.SemanticCacheAPI.UpdateConfig(context.Background()).SemanticCacheConfig(semanticCacheConfig).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SemanticCacheAPI.UpdateConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUpdateConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **semanticCacheConfig** | [**SemanticCacheConfig**](SemanticCacheConfig.md) |  | 

### Return type

 (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

