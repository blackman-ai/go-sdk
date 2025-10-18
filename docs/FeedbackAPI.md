# \FeedbackAPI

All URIs are relative to *https://app.useblackman.ai/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SubmitFeedback**](FeedbackAPI.md#SubmitFeedback) | **Post** /v1/feedback | Submit feedback for a completion response



## SubmitFeedback

> SubmitFeedbackResponse SubmitFeedback(ctx).SubmitFeedbackRequest(submitFeedbackRequest).Execute()

Submit feedback for a completion response

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
	submitFeedbackRequest := *openapiclient.NewSubmitFeedbackRequest(false, "ResponseId_example") // SubmitFeedbackRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.FeedbackAPI.SubmitFeedback(context.Background()).SubmitFeedbackRequest(submitFeedbackRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FeedbackAPI.SubmitFeedback``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SubmitFeedback`: SubmitFeedbackResponse
	fmt.Fprintf(os.Stdout, "Response from `FeedbackAPI.SubmitFeedback`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSubmitFeedbackRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **submitFeedbackRequest** | [**SubmitFeedbackRequest**](SubmitFeedbackRequest.md) |  | 

### Return type

[**SubmitFeedbackResponse**](SubmitFeedbackResponse.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

