# CompletionOptions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MaxTokens** | Pointer to **NullableInt32** |  | [optional] 
**Stop** | Pointer to **[]string** |  | [optional] 
**Stream** | Pointer to **NullableBool** |  | [optional] 
**Temperature** | Pointer to **NullableFloat32** |  | [optional] 
**TopP** | Pointer to **NullableFloat32** |  | [optional] 

## Methods

### NewCompletionOptions

`func NewCompletionOptions() *CompletionOptions`

NewCompletionOptions instantiates a new CompletionOptions object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCompletionOptionsWithDefaults

`func NewCompletionOptionsWithDefaults() *CompletionOptions`

NewCompletionOptionsWithDefaults instantiates a new CompletionOptions object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMaxTokens

`func (o *CompletionOptions) GetMaxTokens() int32`

GetMaxTokens returns the MaxTokens field if non-nil, zero value otherwise.

### GetMaxTokensOk

`func (o *CompletionOptions) GetMaxTokensOk() (*int32, bool)`

GetMaxTokensOk returns a tuple with the MaxTokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxTokens

`func (o *CompletionOptions) SetMaxTokens(v int32)`

SetMaxTokens sets MaxTokens field to given value.

### HasMaxTokens

`func (o *CompletionOptions) HasMaxTokens() bool`

HasMaxTokens returns a boolean if a field has been set.

### SetMaxTokensNil

`func (o *CompletionOptions) SetMaxTokensNil(b bool)`

 SetMaxTokensNil sets the value for MaxTokens to be an explicit nil

### UnsetMaxTokens
`func (o *CompletionOptions) UnsetMaxTokens()`

UnsetMaxTokens ensures that no value is present for MaxTokens, not even an explicit nil
### GetStop

`func (o *CompletionOptions) GetStop() []string`

GetStop returns the Stop field if non-nil, zero value otherwise.

### GetStopOk

`func (o *CompletionOptions) GetStopOk() (*[]string, bool)`

GetStopOk returns a tuple with the Stop field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStop

`func (o *CompletionOptions) SetStop(v []string)`

SetStop sets Stop field to given value.

### HasStop

`func (o *CompletionOptions) HasStop() bool`

HasStop returns a boolean if a field has been set.

### SetStopNil

`func (o *CompletionOptions) SetStopNil(b bool)`

 SetStopNil sets the value for Stop to be an explicit nil

### UnsetStop
`func (o *CompletionOptions) UnsetStop()`

UnsetStop ensures that no value is present for Stop, not even an explicit nil
### GetStream

`func (o *CompletionOptions) GetStream() bool`

GetStream returns the Stream field if non-nil, zero value otherwise.

### GetStreamOk

`func (o *CompletionOptions) GetStreamOk() (*bool, bool)`

GetStreamOk returns a tuple with the Stream field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStream

`func (o *CompletionOptions) SetStream(v bool)`

SetStream sets Stream field to given value.

### HasStream

`func (o *CompletionOptions) HasStream() bool`

HasStream returns a boolean if a field has been set.

### SetStreamNil

`func (o *CompletionOptions) SetStreamNil(b bool)`

 SetStreamNil sets the value for Stream to be an explicit nil

### UnsetStream
`func (o *CompletionOptions) UnsetStream()`

UnsetStream ensures that no value is present for Stream, not even an explicit nil
### GetTemperature

`func (o *CompletionOptions) GetTemperature() float32`

GetTemperature returns the Temperature field if non-nil, zero value otherwise.

### GetTemperatureOk

`func (o *CompletionOptions) GetTemperatureOk() (*float32, bool)`

GetTemperatureOk returns a tuple with the Temperature field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemperature

`func (o *CompletionOptions) SetTemperature(v float32)`

SetTemperature sets Temperature field to given value.

### HasTemperature

`func (o *CompletionOptions) HasTemperature() bool`

HasTemperature returns a boolean if a field has been set.

### SetTemperatureNil

`func (o *CompletionOptions) SetTemperatureNil(b bool)`

 SetTemperatureNil sets the value for Temperature to be an explicit nil

### UnsetTemperature
`func (o *CompletionOptions) UnsetTemperature()`

UnsetTemperature ensures that no value is present for Temperature, not even an explicit nil
### GetTopP

`func (o *CompletionOptions) GetTopP() float32`

GetTopP returns the TopP field if non-nil, zero value otherwise.

### GetTopPOk

`func (o *CompletionOptions) GetTopPOk() (*float32, bool)`

GetTopPOk returns a tuple with the TopP field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTopP

`func (o *CompletionOptions) SetTopP(v float32)`

SetTopP sets TopP field to given value.

### HasTopP

`func (o *CompletionOptions) HasTopP() bool`

HasTopP returns a boolean if a field has been set.

### SetTopPNil

`func (o *CompletionOptions) SetTopPNil(b bool)`

 SetTopPNil sets the value for TopP to be an explicit nil

### UnsetTopP
`func (o *CompletionOptions) UnsetTopP()`

UnsetTopP ensures that no value is present for TopP, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


