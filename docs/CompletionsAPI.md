# \CompletionsAPI

All URIs are relative to *https://app.useblackman.ai/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**Completions**](CompletionsAPI.md#Completions) | **Post** /v1/completions | 



## Completions

> CompletionResponse Completions(ctx).CompletionRequest(completionRequest).XProviderApiKey(xProviderApiKey).Execute()



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
	completionRequest := *openapiclient.NewCompletionRequest([]openapiclient.Message{*openapiclient.NewMessage(openapiclient.MessageContent{ArrayOfContentPart: new([]ContentPart)}, "Role_example")}, "gpt-4", openapiclient.Provider("OpenAI")) // CompletionRequest | 
	xProviderApiKey := "xProviderApiKey_example" // string | Optional provider API key to override stored or system keys (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CompletionsAPI.Completions(context.Background()).CompletionRequest(completionRequest).XProviderApiKey(xProviderApiKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CompletionsAPI.Completions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Completions`: CompletionResponse
	fmt.Fprintf(os.Stdout, "Response from `CompletionsAPI.Completions`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCompletionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **completionRequest** | [**CompletionRequest**](CompletionRequest.md) |  | 
 **xProviderApiKey** | **string** | Optional provider API key to override stored or system keys | 

### Return type

[**CompletionResponse**](CompletionResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

