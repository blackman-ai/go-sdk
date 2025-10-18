# Choice

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FinishReason** | Pointer to **NullableString** |  | [optional] 
**Index** | **int32** |  | 
**Message** | [**Message**](Message.md) |  | 

## Methods

### NewChoice

`func NewChoice(index int32, message Message, ) *Choice`

NewChoice instantiates a new Choice object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewChoiceWithDefaults

`func NewChoiceWithDefaults() *Choice`

NewChoiceWithDefaults instantiates a new Choice object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFinishReason

`func (o *Choice) GetFinishReason() string`

GetFinishReason returns the FinishReason field if non-nil, zero value otherwise.

### GetFinishReasonOk

`func (o *Choice) GetFinishReasonOk() (*string, bool)`

GetFinishReasonOk returns a tuple with the FinishReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFinishReason

`func (o *Choice) SetFinishReason(v string)`

SetFinishReason sets FinishReason field to given value.

### HasFinishReason

`func (o *Choice) HasFinishReason() bool`

HasFinishReason returns a boolean if a field has been set.

### SetFinishReasonNil

`func (o *Choice) SetFinishReasonNil(b bool)`

 SetFinishReasonNil sets the value for FinishReason to be an explicit nil

### UnsetFinishReason
`func (o *Choice) UnsetFinishReason()`

UnsetFinishReason ensures that no value is present for FinishReason, not even an explicit nil
### GetIndex

`func (o *Choice) GetIndex() int32`

GetIndex returns the Index field if non-nil, zero value otherwise.

### GetIndexOk

`func (o *Choice) GetIndexOk() (*int32, bool)`

GetIndexOk returns a tuple with the Index field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndex

`func (o *Choice) SetIndex(v int32)`

SetIndex sets Index field to given value.


### GetMessage

`func (o *Choice) GetMessage() Message`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *Choice) GetMessageOk() (*Message, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *Choice) SetMessage(v Message)`

SetMessage sets Message field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


