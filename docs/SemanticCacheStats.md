# SemanticCacheStats

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AvgSimilarityScore** | **float64** | Average similarity score for cache hits | 
**CostSaved** | **float64** | Total cost saved from cache hits | 
**HitRate** | **float64** | Cache hit rate as a percentage | 
**TokensSaved** | **int64** | Total tokens saved from cache hits | 
**TotalHits** | **int64** | Total number of cache hits | 
**TotalMisses** | **int64** | Total number of cache misses | 

## Methods

### NewSemanticCacheStats

`func NewSemanticCacheStats(avgSimilarityScore float64, costSaved float64, hitRate float64, tokensSaved int64, totalHits int64, totalMisses int64, ) *SemanticCacheStats`

NewSemanticCacheStats instantiates a new SemanticCacheStats object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSemanticCacheStatsWithDefaults

`func NewSemanticCacheStatsWithDefaults() *SemanticCacheStats`

NewSemanticCacheStatsWithDefaults instantiates a new SemanticCacheStats object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAvgSimilarityScore

`func (o *SemanticCacheStats) GetAvgSimilarityScore() float64`

GetAvgSimilarityScore returns the AvgSimilarityScore field if non-nil, zero value otherwise.

### GetAvgSimilarityScoreOk

`func (o *SemanticCacheStats) GetAvgSimilarityScoreOk() (*float64, bool)`

GetAvgSimilarityScoreOk returns a tuple with the AvgSimilarityScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvgSimilarityScore

`func (o *SemanticCacheStats) SetAvgSimilarityScore(v float64)`

SetAvgSimilarityScore sets AvgSimilarityScore field to given value.


### GetCostSaved

`func (o *SemanticCacheStats) GetCostSaved() float64`

GetCostSaved returns the CostSaved field if non-nil, zero value otherwise.

### GetCostSavedOk

`func (o *SemanticCacheStats) GetCostSavedOk() (*float64, bool)`

GetCostSavedOk returns a tuple with the CostSaved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCostSaved

`func (o *SemanticCacheStats) SetCostSaved(v float64)`

SetCostSaved sets CostSaved field to given value.


### GetHitRate

`func (o *SemanticCacheStats) GetHitRate() float64`

GetHitRate returns the HitRate field if non-nil, zero value otherwise.

### GetHitRateOk

`func (o *SemanticCacheStats) GetHitRateOk() (*float64, bool)`

GetHitRateOk returns a tuple with the HitRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHitRate

`func (o *SemanticCacheStats) SetHitRate(v float64)`

SetHitRate sets HitRate field to given value.


### GetTokensSaved

`func (o *SemanticCacheStats) GetTokensSaved() int64`

GetTokensSaved returns the TokensSaved field if non-nil, zero value otherwise.

### GetTokensSavedOk

`func (o *SemanticCacheStats) GetTokensSavedOk() (*int64, bool)`

GetTokensSavedOk returns a tuple with the TokensSaved field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokensSaved

`func (o *SemanticCacheStats) SetTokensSaved(v int64)`

SetTokensSaved sets TokensSaved field to given value.


### GetTotalHits

`func (o *SemanticCacheStats) GetTotalHits() int64`

GetTotalHits returns the TotalHits field if non-nil, zero value otherwise.

### GetTotalHitsOk

`func (o *SemanticCacheStats) GetTotalHitsOk() (*int64, bool)`

GetTotalHitsOk returns a tuple with the TotalHits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalHits

`func (o *SemanticCacheStats) SetTotalHits(v int64)`

SetTotalHits sets TotalHits field to given value.


### GetTotalMisses

`func (o *SemanticCacheStats) GetTotalMisses() int64`

GetTotalMisses returns the TotalMisses field if non-nil, zero value otherwise.

### GetTotalMissesOk

`func (o *SemanticCacheStats) GetTotalMissesOk() (*int64, bool)`

GetTotalMissesOk returns a tuple with the TotalMisses field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalMisses

`func (o *SemanticCacheStats) SetTotalMisses(v int64)`

SetTotalMisses sets TotalMisses field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


