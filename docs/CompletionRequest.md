# CompletionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MaxTokens** | Pointer to **NullableInt32** |  | [optional] 
**Stop** | Pointer to **[]string** |  | [optional] 
**Stream** | Pointer to **NullableBool** |  | [optional] 
**Temperature** | Pointer to **NullableFloat32** |  | [optional] 
**TopP** | Pointer to **NullableFloat32** |  | [optional] 
**Messages** | [**[]Message**](Message.md) |  | 
**Model** | **string** |  | 
**Provider** | [**Provider**](Provider.md) |  | 

## Methods

### NewCompletionRequest

`func NewCompletionRequest(messages []Message, model string, provider Provider, ) *CompletionRequest`

NewCompletionRequest instantiates a new CompletionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCompletionRequestWithDefaults

`func NewCompletionRequestWithDefaults() *CompletionRequest`

NewCompletionRequestWithDefaults instantiates a new CompletionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMaxTokens

`func (o *CompletionRequest) GetMaxTokens() int32`

GetMaxTokens returns the MaxTokens field if non-nil, zero value otherwise.

### GetMaxTokensOk

`func (o *CompletionRequest) GetMaxTokensOk() (*int32, bool)`

GetMaxTokensOk returns a tuple with the MaxTokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxTokens

`func (o *CompletionRequest) SetMaxTokens(v int32)`

SetMaxTokens sets MaxTokens field to given value.

### HasMaxTokens

`func (o *CompletionRequest) HasMaxTokens() bool`

HasMaxTokens returns a boolean if a field has been set.

### SetMaxTokensNil

`func (o *CompletionRequest) SetMaxTokensNil(b bool)`

 SetMaxTokensNil sets the value for MaxTokens to be an explicit nil

### UnsetMaxTokens
`func (o *CompletionRequest) UnsetMaxTokens()`

UnsetMaxTokens ensures that no value is present for MaxTokens, not even an explicit nil
### GetStop

`func (o *CompletionRequest) GetStop() []string`

GetStop returns the Stop field if non-nil, zero value otherwise.

### GetStopOk

`func (o *CompletionRequest) GetStopOk() (*[]string, bool)`

GetStopOk returns a tuple with the Stop field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStop

`func (o *CompletionRequest) SetStop(v []string)`

SetStop sets Stop field to given value.

### HasStop

`func (o *CompletionRequest) HasStop() bool`

HasStop returns a boolean if a field has been set.

### SetStopNil

`func (o *CompletionRequest) SetStopNil(b bool)`

 SetStopNil sets the value for Stop to be an explicit nil

### UnsetStop
`func (o *CompletionRequest) UnsetStop()`

UnsetStop ensures that no value is present for Stop, not even an explicit nil
### GetStream

`func (o *CompletionRequest) GetStream() bool`

GetStream returns the Stream field if non-nil, zero value otherwise.

### GetStreamOk

`func (o *CompletionRequest) GetStreamOk() (*bool, bool)`

GetStreamOk returns a tuple with the Stream field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStream

`func (o *CompletionRequest) SetStream(v bool)`

SetStream sets Stream field to given value.

### HasStream

`func (o *CompletionRequest) HasStream() bool`

HasStream returns a boolean if a field has been set.

### SetStreamNil

`func (o *CompletionRequest) SetStreamNil(b bool)`

 SetStreamNil sets the value for Stream to be an explicit nil

### UnsetStream
`func (o *CompletionRequest) UnsetStream()`

UnsetStream ensures that no value is present for Stream, not even an explicit nil
### GetTemperature

`func (o *CompletionRequest) GetTemperature() float32`

GetTemperature returns the Temperature field if non-nil, zero value otherwise.

### GetTemperatureOk

`func (o *CompletionRequest) GetTemperatureOk() (*float32, bool)`

GetTemperatureOk returns a tuple with the Temperature field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemperature

`func (o *CompletionRequest) SetTemperature(v float32)`

SetTemperature sets Temperature field to given value.

### HasTemperature

`func (o *CompletionRequest) HasTemperature() bool`

HasTemperature returns a boolean if a field has been set.

### SetTemperatureNil

`func (o *CompletionRequest) SetTemperatureNil(b bool)`

 SetTemperatureNil sets the value for Temperature to be an explicit nil

### UnsetTemperature
`func (o *CompletionRequest) UnsetTemperature()`

UnsetTemperature ensures that no value is present for Temperature, not even an explicit nil
### GetTopP

`func (o *CompletionRequest) GetTopP() float32`

GetTopP returns the TopP field if non-nil, zero value otherwise.

### GetTopPOk

`func (o *CompletionRequest) GetTopPOk() (*float32, bool)`

GetTopPOk returns a tuple with the TopP field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTopP

`func (o *CompletionRequest) SetTopP(v float32)`

SetTopP sets TopP field to given value.

### HasTopP

`func (o *CompletionRequest) HasTopP() bool`

HasTopP returns a boolean if a field has been set.

### SetTopPNil

`func (o *CompletionRequest) SetTopPNil(b bool)`

 SetTopPNil sets the value for TopP to be an explicit nil

### UnsetTopP
`func (o *CompletionRequest) UnsetTopP()`

UnsetTopP ensures that no value is present for TopP, not even an explicit nil
### GetMessages

`func (o *CompletionRequest) GetMessages() []Message`

GetMessages returns the Messages field if non-nil, zero value otherwise.

### GetMessagesOk

`func (o *CompletionRequest) GetMessagesOk() (*[]Message, bool)`

GetMessagesOk returns a tuple with the Messages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessages

`func (o *CompletionRequest) SetMessages(v []Message)`

SetMessages sets Messages field to given value.


### GetModel

`func (o *CompletionRequest) GetModel() string`

GetModel returns the Model field if non-nil, zero value otherwise.

### GetModelOk

`func (o *CompletionRequest) GetModelOk() (*string, bool)`

GetModelOk returns a tuple with the Model field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModel

`func (o *CompletionRequest) SetModel(v string)`

SetModel sets Model field to given value.


### GetProvider

`func (o *CompletionRequest) GetProvider() Provider`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *CompletionRequest) GetProviderOk() (*Provider, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *CompletionRequest) SetProvider(v Provider)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


