# CompletionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Choices** | [**[]Choice**](Choice.md) |  | 
**Created** | **int64** |  | 
**Id** | **string** |  | 
**Model** | **string** |  | 
**Provider** | [**Provider**](Provider.md) |  | 
**Usage** | [**Usage**](Usage.md) |  | 

## Methods

### NewCompletionResponse

`func NewCompletionResponse(choices []Choice, created int64, id string, model string, provider Provider, usage Usage, ) *CompletionResponse`

NewCompletionResponse instantiates a new CompletionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCompletionResponseWithDefaults

`func NewCompletionResponseWithDefaults() *CompletionResponse`

NewCompletionResponseWithDefaults instantiates a new CompletionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChoices

`func (o *CompletionResponse) GetChoices() []Choice`

GetChoices returns the Choices field if non-nil, zero value otherwise.

### GetChoicesOk

`func (o *CompletionResponse) GetChoicesOk() (*[]Choice, bool)`

GetChoicesOk returns a tuple with the Choices field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChoices

`func (o *CompletionResponse) SetChoices(v []Choice)`

SetChoices sets Choices field to given value.


### GetCreated

`func (o *CompletionResponse) GetCreated() int64`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *CompletionResponse) GetCreatedOk() (*int64, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *CompletionResponse) SetCreated(v int64)`

SetCreated sets Created field to given value.


### GetId

`func (o *CompletionResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *CompletionResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *CompletionResponse) SetId(v string)`

SetId sets Id field to given value.


### GetModel

`func (o *CompletionResponse) GetModel() string`

GetModel returns the Model field if non-nil, zero value otherwise.

### GetModelOk

`func (o *CompletionResponse) GetModelOk() (*string, bool)`

GetModelOk returns a tuple with the Model field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModel

`func (o *CompletionResponse) SetModel(v string)`

SetModel sets Model field to given value.


### GetProvider

`func (o *CompletionResponse) GetProvider() Provider`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *CompletionResponse) GetProviderOk() (*Provider, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *CompletionResponse) SetProvider(v Provider)`

SetProvider sets Provider field to given value.


### GetUsage

`func (o *CompletionResponse) GetUsage() Usage`

GetUsage returns the Usage field if non-nil, zero value otherwise.

### GetUsageOk

`func (o *CompletionResponse) GetUsageOk() (*Usage, bool)`

GetUsageOk returns a tuple with the Usage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsage

`func (o *CompletionResponse) SetUsage(v Usage)`

SetUsage sets Usage field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


