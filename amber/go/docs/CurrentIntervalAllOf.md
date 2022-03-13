# CurrentIntervalAllOf

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** |  | [optional] 
**Range** | Pointer to [**NullableForecastIntervalAllOfRange**](ForecastIntervalAllOfRange.md) |  | [optional] 
**Estimate** | **bool** | Shows true the current price is an estimate. Shows false is the price has been locked in. | 

## Methods

### NewCurrentIntervalAllOf

`func NewCurrentIntervalAllOf(estimate bool, ) *CurrentIntervalAllOf`

NewCurrentIntervalAllOf instantiates a new CurrentIntervalAllOf object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCurrentIntervalAllOfWithDefaults

`func NewCurrentIntervalAllOfWithDefaults() *CurrentIntervalAllOf`

NewCurrentIntervalAllOfWithDefaults instantiates a new CurrentIntervalAllOf object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *CurrentIntervalAllOf) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CurrentIntervalAllOf) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CurrentIntervalAllOf) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *CurrentIntervalAllOf) HasType() bool`

HasType returns a boolean if a field has been set.

### GetRange

`func (o *CurrentIntervalAllOf) GetRange() ForecastIntervalAllOfRange`

GetRange returns the Range field if non-nil, zero value otherwise.

### GetRangeOk

`func (o *CurrentIntervalAllOf) GetRangeOk() (*ForecastIntervalAllOfRange, bool)`

GetRangeOk returns a tuple with the Range field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRange

`func (o *CurrentIntervalAllOf) SetRange(v ForecastIntervalAllOfRange)`

SetRange sets Range field to given value.

### HasRange

`func (o *CurrentIntervalAllOf) HasRange() bool`

HasRange returns a boolean if a field has been set.

### SetRangeNil

`func (o *CurrentIntervalAllOf) SetRangeNil(b bool)`

 SetRangeNil sets the value for Range to be an explicit nil

### UnsetRange
`func (o *CurrentIntervalAllOf) UnsetRange()`

UnsetRange ensures that no value is present for Range, not even an explicit nil
### GetEstimate

`func (o *CurrentIntervalAllOf) GetEstimate() bool`

GetEstimate returns the Estimate field if non-nil, zero value otherwise.

### GetEstimateOk

`func (o *CurrentIntervalAllOf) GetEstimateOk() (*bool, bool)`

GetEstimateOk returns a tuple with the Estimate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEstimate

`func (o *CurrentIntervalAllOf) SetEstimate(v bool)`

SetEstimate sets Estimate field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


