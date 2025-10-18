# SubmitFeedbackRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IsPositive** | **bool** | True for thumbs up, false for thumbs down | 
**Metadata** | Pointer to **map[string]interface{}** | Optional metadata (e.g., user_agent, session_id, etc.) | [optional] 
**ResponseId** | **string** | The response ID from the completion request | 

## Methods

### NewSubmitFeedbackRequest

`func NewSubmitFeedbackRequest(isPositive bool, responseId string, ) *SubmitFeedbackRequest`

NewSubmitFeedbackRequest instantiates a new SubmitFeedbackRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSubmitFeedbackRequestWithDefaults

`func NewSubmitFeedbackRequestWithDefaults() *SubmitFeedbackRequest`

NewSubmitFeedbackRequestWithDefaults instantiates a new SubmitFeedbackRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIsPositive

`func (o *SubmitFeedbackRequest) GetIsPositive() bool`

GetIsPositive returns the IsPositive field if non-nil, zero value otherwise.

### GetIsPositiveOk

`func (o *SubmitFeedbackRequest) GetIsPositiveOk() (*bool, bool)`

GetIsPositiveOk returns a tuple with the IsPositive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsPositive

`func (o *SubmitFeedbackRequest) SetIsPositive(v bool)`

SetIsPositive sets IsPositive field to given value.


### GetMetadata

`func (o *SubmitFeedbackRequest) GetMetadata() map[string]interface{}`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *SubmitFeedbackRequest) GetMetadataOk() (*map[string]interface{}, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *SubmitFeedbackRequest) SetMetadata(v map[string]interface{})`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *SubmitFeedbackRequest) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### SetMetadataNil

`func (o *SubmitFeedbackRequest) SetMetadataNil(b bool)`

 SetMetadataNil sets the value for Metadata to be an explicit nil

### UnsetMetadata
`func (o *SubmitFeedbackRequest) UnsetMetadata()`

UnsetMetadata ensures that no value is present for Metadata, not even an explicit nil
### GetResponseId

`func (o *SubmitFeedbackRequest) GetResponseId() string`

GetResponseId returns the ResponseId field if non-nil, zero value otherwise.

### GetResponseIdOk

`func (o *SubmitFeedbackRequest) GetResponseIdOk() (*string, bool)`

GetResponseIdOk returns a tuple with the ResponseId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseId

`func (o *SubmitFeedbackRequest) SetResponseId(v string)`

SetResponseId sets ResponseId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


