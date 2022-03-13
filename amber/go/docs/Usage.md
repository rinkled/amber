# Usage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Duration** | **float32** | Length of the interval in minutes. | 
**SpotPerKwh** | **float32** | NEM spot price (c/kWh). This is the price generators get paid to generate electricity, and what drives the variable component of your perKwh price - includes GST | 
**PerKwh** | **float32** | Number of cents you will pay per kilowatt-hour (c/kWh) - includes GST | 
**Date** | **string** | Date the interval belongs to (in NEM time). This may be different to the date component of nemTime, as the last interval of the day ends at 12:00 the following day. Formatted as a ISO 8601 date | 
**NemTime** | **time.Time** | The interval&#39;s NEM time. This represents the time at the end of the interval UTC+10. Formatted as a ISO 8601 time | 
**StartTime** | **time.Time** | Start time of the interval in UTC. Formatted as a ISO 8601 time | 
**EndTime** | **time.Time** | End time of the interval in UTC. Formatted as a ISO 8601 time | 
**Renewables** | **float32** | Percentage of renewables in the grid | 
**ChannelType** | **string** | Meter channel type | 
**TariffInformation** | Pointer to [**NullableIntervalTariffInformation**](IntervalTariffInformation.md) |  | [optional] 
**SpikeStatus** | **string** | Indicates whether this interval will potentially spike, or is currently in a spike state | 
**Descriptor** | Pointer to **string** | Describes the current price. Gives you an indication of how cheap the price is in relation to the average VMO and DMO. Note: Negative is no longer used. It has been replaced with extremelyLow. | [optional] 
**ChannelIdentifier** | Pointer to **string** | Meter channel identifier | [optional] 
**Kwh** | **float32** | Number of kWh you consumed or generated. Generated numbers will be negative | 
**Quality** | **string** | If the metering company has had trouble contacting your meter, they may make an estimate of your usage for that period. Billable data is data that will appear on your bill. | 
**Cost** | **float32** | The total cost of your consumption or generation for this period - includes GST | 

## Methods

### NewUsage

`func NewUsage(type_ string, duration float32, spotPerKwh float32, perKwh float32, date string, nemTime time.Time, startTime time.Time, endTime time.Time, renewables float32, channelType string, spikeStatus string, kwh float32, quality string, cost float32, ) *Usage`

NewUsage instantiates a new Usage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsageWithDefaults

`func NewUsageWithDefaults() *Usage`

NewUsageWithDefaults instantiates a new Usage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *Usage) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Usage) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Usage) SetType(v string)`

SetType sets Type field to given value.


### GetDuration

`func (o *Usage) GetDuration() float32`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *Usage) GetDurationOk() (*float32, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *Usage) SetDuration(v float32)`

SetDuration sets Duration field to given value.


### GetSpotPerKwh

`func (o *Usage) GetSpotPerKwh() float32`

GetSpotPerKwh returns the SpotPerKwh field if non-nil, zero value otherwise.

### GetSpotPerKwhOk

`func (o *Usage) GetSpotPerKwhOk() (*float32, bool)`

GetSpotPerKwhOk returns a tuple with the SpotPerKwh field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpotPerKwh

`func (o *Usage) SetSpotPerKwh(v float32)`

SetSpotPerKwh sets SpotPerKwh field to given value.


### GetPerKwh

`func (o *Usage) GetPerKwh() float32`

GetPerKwh returns the PerKwh field if non-nil, zero value otherwise.

### GetPerKwhOk

`func (o *Usage) GetPerKwhOk() (*float32, bool)`

GetPerKwhOk returns a tuple with the PerKwh field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPerKwh

`func (o *Usage) SetPerKwh(v float32)`

SetPerKwh sets PerKwh field to given value.


### GetDate

`func (o *Usage) GetDate() string`

GetDate returns the Date field if non-nil, zero value otherwise.

### GetDateOk

`func (o *Usage) GetDateOk() (*string, bool)`

GetDateOk returns a tuple with the Date field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDate

`func (o *Usage) SetDate(v string)`

SetDate sets Date field to given value.


### GetNemTime

`func (o *Usage) GetNemTime() time.Time`

GetNemTime returns the NemTime field if non-nil, zero value otherwise.

### GetNemTimeOk

`func (o *Usage) GetNemTimeOk() (*time.Time, bool)`

GetNemTimeOk returns a tuple with the NemTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNemTime

`func (o *Usage) SetNemTime(v time.Time)`

SetNemTime sets NemTime field to given value.


### GetStartTime

`func (o *Usage) GetStartTime() time.Time`

GetStartTime returns the StartTime field if non-nil, zero value otherwise.

### GetStartTimeOk

`func (o *Usage) GetStartTimeOk() (*time.Time, bool)`

GetStartTimeOk returns a tuple with the StartTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartTime

`func (o *Usage) SetStartTime(v time.Time)`

SetStartTime sets StartTime field to given value.


### GetEndTime

`func (o *Usage) GetEndTime() time.Time`

GetEndTime returns the EndTime field if non-nil, zero value otherwise.

### GetEndTimeOk

`func (o *Usage) GetEndTimeOk() (*time.Time, bool)`

GetEndTimeOk returns a tuple with the EndTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndTime

`func (o *Usage) SetEndTime(v time.Time)`

SetEndTime sets EndTime field to given value.


### GetRenewables

`func (o *Usage) GetRenewables() float32`

GetRenewables returns the Renewables field if non-nil, zero value otherwise.

### GetRenewablesOk

`func (o *Usage) GetRenewablesOk() (*float32, bool)`

GetRenewablesOk returns a tuple with the Renewables field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenewables

`func (o *Usage) SetRenewables(v float32)`

SetRenewables sets Renewables field to given value.


### GetChannelType

`func (o *Usage) GetChannelType() string`

GetChannelType returns the ChannelType field if non-nil, zero value otherwise.

### GetChannelTypeOk

`func (o *Usage) GetChannelTypeOk() (*string, bool)`

GetChannelTypeOk returns a tuple with the ChannelType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannelType

`func (o *Usage) SetChannelType(v string)`

SetChannelType sets ChannelType field to given value.


### GetTariffInformation

`func (o *Usage) GetTariffInformation() IntervalTariffInformation`

GetTariffInformation returns the TariffInformation field if non-nil, zero value otherwise.

### GetTariffInformationOk

`func (o *Usage) GetTariffInformationOk() (*IntervalTariffInformation, bool)`

GetTariffInformationOk returns a tuple with the TariffInformation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTariffInformation

`func (o *Usage) SetTariffInformation(v IntervalTariffInformation)`

SetTariffInformation sets TariffInformation field to given value.

### HasTariffInformation

`func (o *Usage) HasTariffInformation() bool`

HasTariffInformation returns a boolean if a field has been set.

### SetTariffInformationNil

`func (o *Usage) SetTariffInformationNil(b bool)`

 SetTariffInformationNil sets the value for TariffInformation to be an explicit nil

### UnsetTariffInformation
`func (o *Usage) UnsetTariffInformation()`

UnsetTariffInformation ensures that no value is present for TariffInformation, not even an explicit nil
### GetSpikeStatus

`func (o *Usage) GetSpikeStatus() string`

GetSpikeStatus returns the SpikeStatus field if non-nil, zero value otherwise.

### GetSpikeStatusOk

`func (o *Usage) GetSpikeStatusOk() (*string, bool)`

GetSpikeStatusOk returns a tuple with the SpikeStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSpikeStatus

`func (o *Usage) SetSpikeStatus(v string)`

SetSpikeStatus sets SpikeStatus field to given value.


### GetDescriptor

`func (o *Usage) GetDescriptor() string`

GetDescriptor returns the Descriptor field if non-nil, zero value otherwise.

### GetDescriptorOk

`func (o *Usage) GetDescriptorOk() (*string, bool)`

GetDescriptorOk returns a tuple with the Descriptor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescriptor

`func (o *Usage) SetDescriptor(v string)`

SetDescriptor sets Descriptor field to given value.

### HasDescriptor

`func (o *Usage) HasDescriptor() bool`

HasDescriptor returns a boolean if a field has been set.

### GetChannelIdentifier

`func (o *Usage) GetChannelIdentifier() string`

GetChannelIdentifier returns the ChannelIdentifier field if non-nil, zero value otherwise.

### GetChannelIdentifierOk

`func (o *Usage) GetChannelIdentifierOk() (*string, bool)`

GetChannelIdentifierOk returns a tuple with the ChannelIdentifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannelIdentifier

`func (o *Usage) SetChannelIdentifier(v string)`

SetChannelIdentifier sets ChannelIdentifier field to given value.

### HasChannelIdentifier

`func (o *Usage) HasChannelIdentifier() bool`

HasChannelIdentifier returns a boolean if a field has been set.

### GetKwh

`func (o *Usage) GetKwh() float32`

GetKwh returns the Kwh field if non-nil, zero value otherwise.

### GetKwhOk

`func (o *Usage) GetKwhOk() (*float32, bool)`

GetKwhOk returns a tuple with the Kwh field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKwh

`func (o *Usage) SetKwh(v float32)`

SetKwh sets Kwh field to given value.


### GetQuality

`func (o *Usage) GetQuality() string`

GetQuality returns the Quality field if non-nil, zero value otherwise.

### GetQualityOk

`func (o *Usage) GetQualityOk() (*string, bool)`

GetQualityOk returns a tuple with the Quality field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuality

`func (o *Usage) SetQuality(v string)`

SetQuality sets Quality field to given value.


### GetCost

`func (o *Usage) GetCost() float32`

GetCost returns the Cost field if non-nil, zero value otherwise.

### GetCostOk

`func (o *Usage) GetCostOk() (*float32, bool)`

GetCostOk returns a tuple with the Cost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCost

`func (o *Usage) SetCost(v float32)`

SetCost sets Cost field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


