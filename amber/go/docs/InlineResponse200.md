# InlineResponse200

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Unique Site Identifier | 
**Nmi** | **string** | National Metering Identifier (NMI) for the site | 
**Channels** | [**[]SitesChannels**](SitesChannels.md) | List of channels that are readable from your meter | 
**Network** | **string** | The name of the site&#39;s network | 

## Methods

### NewInlineResponse200

`func NewInlineResponse200(id string, nmi string, channels []SitesChannels, network string, ) *InlineResponse200`

NewInlineResponse200 instantiates a new InlineResponse200 object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInlineResponse200WithDefaults

`func NewInlineResponse200WithDefaults() *InlineResponse200`

NewInlineResponse200WithDefaults instantiates a new InlineResponse200 object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InlineResponse200) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InlineResponse200) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InlineResponse200) SetId(v string)`

SetId sets Id field to given value.


### GetNmi

`func (o *InlineResponse200) GetNmi() string`

GetNmi returns the Nmi field if non-nil, zero value otherwise.

### GetNmiOk

`func (o *InlineResponse200) GetNmiOk() (*string, bool)`

GetNmiOk returns a tuple with the Nmi field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNmi

`func (o *InlineResponse200) SetNmi(v string)`

SetNmi sets Nmi field to given value.


### GetChannels

`func (o *InlineResponse200) GetChannels() []SitesChannels`

GetChannels returns the Channels field if non-nil, zero value otherwise.

### GetChannelsOk

`func (o *InlineResponse200) GetChannelsOk() (*[]SitesChannels, bool)`

GetChannelsOk returns a tuple with the Channels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannels

`func (o *InlineResponse200) SetChannels(v []SitesChannels)`

SetChannels sets Channels field to given value.


### GetNetwork

`func (o *InlineResponse200) GetNetwork() string`

GetNetwork returns the Network field if non-nil, zero value otherwise.

### GetNetworkOk

`func (o *InlineResponse200) GetNetworkOk() (*string, bool)`

GetNetworkOk returns a tuple with the Network field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetwork

`func (o *InlineResponse200) SetNetwork(v string)`

SetNetwork sets Network field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


