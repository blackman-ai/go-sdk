# ContentPart

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Text** | **string** |  | 
**Type** | **string** |  | 
**ImageUrl** | [**ImageUrl**](ImageUrl.md) |  | 

## Methods

### NewContentPart

`func NewContentPart(text string, type_ string, imageUrl ImageUrl, ) *ContentPart`

NewContentPart instantiates a new ContentPart object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewContentPartWithDefaults

`func NewContentPartWithDefaults() *ContentPart`

NewContentPartWithDefaults instantiates a new ContentPart object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetText

`func (o *ContentPart) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *ContentPart) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *ContentPart) SetText(v string)`

SetText sets Text field to given value.


### GetType

`func (o *ContentPart) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ContentPart) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ContentPart) SetType(v string)`

SetType sets Type field to given value.


### GetImageUrl

`func (o *ContentPart) GetImageUrl() ImageUrl`

GetImageUrl returns the ImageUrl field if non-nil, zero value otherwise.

### GetImageUrlOk

`func (o *ContentPart) GetImageUrlOk() (*ImageUrl, bool)`

GetImageUrlOk returns a tuple with the ImageUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImageUrl

`func (o *ContentPart) SetImageUrl(v ImageUrl)`

SetImageUrl sets ImageUrl field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


