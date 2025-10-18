# SemanticCacheConfig

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether semantic caching is enabled | 
**SimilarityThreshold** | **float64** | Similarity threshold for cache hits (0.0-1.0) | 
**TtlSeconds** | **int64** | Time-to-live for cache entries in seconds | 

## Methods

### NewSemanticCacheConfig

`func NewSemanticCacheConfig(enabled bool, similarityThreshold float64, ttlSeconds int64, ) *SemanticCacheConfig`

NewSemanticCacheConfig instantiates a new SemanticCacheConfig object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSemanticCacheConfigWithDefaults

`func NewSemanticCacheConfigWithDefaults() *SemanticCacheConfig`

NewSemanticCacheConfigWithDefaults instantiates a new SemanticCacheConfig object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *SemanticCacheConfig) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *SemanticCacheConfig) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *SemanticCacheConfig) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetSimilarityThreshold

`func (o *SemanticCacheConfig) GetSimilarityThreshold() float64`

GetSimilarityThreshold returns the SimilarityThreshold field if non-nil, zero value otherwise.

### GetSimilarityThresholdOk

`func (o *SemanticCacheConfig) GetSimilarityThresholdOk() (*float64, bool)`

GetSimilarityThresholdOk returns a tuple with the SimilarityThreshold field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSimilarityThreshold

`func (o *SemanticCacheConfig) SetSimilarityThreshold(v float64)`

SetSimilarityThreshold sets SimilarityThreshold field to given value.


### GetTtlSeconds

`func (o *SemanticCacheConfig) GetTtlSeconds() int64`

GetTtlSeconds returns the TtlSeconds field if non-nil, zero value otherwise.

### GetTtlSecondsOk

`func (o *SemanticCacheConfig) GetTtlSecondsOk() (*int64, bool)`

GetTtlSecondsOk returns a tuple with the TtlSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTtlSeconds

`func (o *SemanticCacheConfig) SetTtlSeconds(v int64)`

SetTtlSeconds sets TtlSeconds field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


