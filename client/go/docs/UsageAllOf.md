# UsageAllOf

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** |  | [optional] 
**ChannelIdentifier** | Pointer to **string** | Meter channel identifier | [optional] 
**Kwh** | **float32** | Number of kWh you consumed or generated. Generated numbers will be negative | 
**Quality** | **string** | If the metering company has had trouble contacting your meter, they may make an estimate of your usage for that period. Billable data is data that will appear on your bill. | 
**Cost** | **float32** | The total cost of your consumption or generation for this period - includes GST | 

## Methods

### NewUsageAllOf

`func NewUsageAllOf(kwh float32, quality string, cost float32, ) *UsageAllOf`

NewUsageAllOf instantiates a new UsageAllOf object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsageAllOfWithDefaults

`func NewUsageAllOfWithDefaults() *UsageAllOf`

NewUsageAllOfWithDefaults instantiates a new UsageAllOf object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *UsageAllOf) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *UsageAllOf) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *UsageAllOf) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *UsageAllOf) HasType() bool`

HasType returns a boolean if a field has been set.

### GetChannelIdentifier

`func (o *UsageAllOf) GetChannelIdentifier() string`

GetChannelIdentifier returns the ChannelIdentifier field if non-nil, zero value otherwise.

### GetChannelIdentifierOk

`func (o *UsageAllOf) GetChannelIdentifierOk() (*string, bool)`

GetChannelIdentifierOk returns a tuple with the ChannelIdentifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannelIdentifier

`func (o *UsageAllOf) SetChannelIdentifier(v string)`

SetChannelIdentifier sets ChannelIdentifier field to given value.

### HasChannelIdentifier

`func (o *UsageAllOf) HasChannelIdentifier() bool`

HasChannelIdentifier returns a boolean if a field has been set.

### GetKwh

`func (o *UsageAllOf) GetKwh() float32`

GetKwh returns the Kwh field if non-nil, zero value otherwise.

### GetKwhOk

`func (o *UsageAllOf) GetKwhOk() (*float32, bool)`

GetKwhOk returns a tuple with the Kwh field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKwh

`func (o *UsageAllOf) SetKwh(v float32)`

SetKwh sets Kwh field to given value.


### GetQuality

`func (o *UsageAllOf) GetQuality() string`

GetQuality returns the Quality field if non-nil, zero value otherwise.

### GetQualityOk

`func (o *UsageAllOf) GetQualityOk() (*string, bool)`

GetQualityOk returns a tuple with the Quality field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuality

`func (o *UsageAllOf) SetQuality(v string)`

SetQuality sets Quality field to given value.


### GetCost

`func (o *UsageAllOf) GetCost() float32`

GetCost returns the Cost field if non-nil, zero value otherwise.

### GetCostOk

`func (o *UsageAllOf) GetCostOk() (*float32, bool)`

GetCostOk returns a tuple with the Cost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCost

`func (o *UsageAllOf) SetCost(v float32)`

SetCost sets Cost field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


