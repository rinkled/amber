# IntervalTariffInformation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Period** | Pointer to **string** | The Time of Use period that is currently active. Only available if the site in on a time of use tariff | [optional] 
**Season** | Pointer to **string** | The Time of Use season that is currently active. Only available if the site in on a time of use tariff | [optional] 
**Block** | Pointer to **float32** | The block that is currently active. Only available in the site in on a block tariff | [optional] 
**DemandWindow** | Pointer to **bool** | Is this interval currently in the demand window? Only available if the site in on a demand tariff | [optional] 

## Methods

### NewIntervalTariffInformation

`func NewIntervalTariffInformation() *IntervalTariffInformation`

NewIntervalTariffInformation instantiates a new IntervalTariffInformation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIntervalTariffInformationWithDefaults

`func NewIntervalTariffInformationWithDefaults() *IntervalTariffInformation`

NewIntervalTariffInformationWithDefaults instantiates a new IntervalTariffInformation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPeriod

`func (o *IntervalTariffInformation) GetPeriod() string`

GetPeriod returns the Period field if non-nil, zero value otherwise.

### GetPeriodOk

`func (o *IntervalTariffInformation) GetPeriodOk() (*string, bool)`

GetPeriodOk returns a tuple with the Period field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPeriod

`func (o *IntervalTariffInformation) SetPeriod(v string)`

SetPeriod sets Period field to given value.

### HasPeriod

`func (o *IntervalTariffInformation) HasPeriod() bool`

HasPeriod returns a boolean if a field has been set.

### GetSeason

`func (o *IntervalTariffInformation) GetSeason() string`

GetSeason returns the Season field if non-nil, zero value otherwise.

### GetSeasonOk

`func (o *IntervalTariffInformation) GetSeasonOk() (*string, bool)`

GetSeasonOk returns a tuple with the Season field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeason

`func (o *IntervalTariffInformation) SetSeason(v string)`

SetSeason sets Season field to given value.

### HasSeason

`func (o *IntervalTariffInformation) HasSeason() bool`

HasSeason returns a boolean if a field has been set.

### GetBlock

`func (o *IntervalTariffInformation) GetBlock() float32`

GetBlock returns the Block field if non-nil, zero value otherwise.

### GetBlockOk

`func (o *IntervalTariffInformation) GetBlockOk() (*float32, bool)`

GetBlockOk returns a tuple with the Block field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlock

`func (o *IntervalTariffInformation) SetBlock(v float32)`

SetBlock sets Block field to given value.

### HasBlock

`func (o *IntervalTariffInformation) HasBlock() bool`

HasBlock returns a boolean if a field has been set.

### GetDemandWindow

`func (o *IntervalTariffInformation) GetDemandWindow() bool`

GetDemandWindow returns the DemandWindow field if non-nil, zero value otherwise.

### GetDemandWindowOk

`func (o *IntervalTariffInformation) GetDemandWindowOk() (*bool, bool)`

GetDemandWindowOk returns a tuple with the DemandWindow field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDemandWindow

`func (o *IntervalTariffInformation) SetDemandWindow(v bool)`

SetDemandWindow sets DemandWindow field to given value.

### HasDemandWindow

`func (o *IntervalTariffInformation) HasDemandWindow() bool`

HasDemandWindow returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


