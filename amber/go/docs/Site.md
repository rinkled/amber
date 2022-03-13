# Site

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Unique Site Identifier | 
**Nmi** | **string** | National Metering Identifier (NMI) for the site | 
**Channels** | [**[]SitesChannels**](SitesChannels.md) | List of channels that are readable from your meter | 
**Network** | **string** | The name of the site&#39;s network | 

## Methods

### NewSite

`func NewSite(id string, nmi string, channels []SitesChannels, network string, ) *Site`

NewSite instantiates a new Site object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSiteWithDefaults

`func NewSiteWithDefaults() *Site`

NewSiteWithDefaults instantiates a new Site object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Site) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Site) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Site) SetId(v string)`

SetId sets Id field to given value.


### GetNmi

`func (o *Site) GetNmi() string`

GetNmi returns the Nmi field if non-nil, zero value otherwise.

### GetNmiOk

`func (o *Site) GetNmiOk() (*string, bool)`

GetNmiOk returns a tuple with the Nmi field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNmi

`func (o *Site) SetNmi(v string)`

SetNmi sets Nmi field to given value.


### GetChannels

`func (o *Site) GetChannels() []SitesChannels`

GetChannels returns the Channels field if non-nil, zero value otherwise.

### GetChannelsOk

`func (o *Site) GetChannelsOk() (*[]SitesChannels, bool)`

GetChannelsOk returns a tuple with the Channels field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannels

`func (o *Site) SetChannels(v []SitesChannels)`

SetChannels sets Channels field to given value.


### GetNetwork

`func (o *Site) GetNetwork() string`

GetNetwork returns the Network field if non-nil, zero value otherwise.

### GetNetworkOk

`func (o *Site) GetNetworkOk() (*string, bool)`

GetNetworkOk returns a tuple with the Network field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetwork

`func (o *Site) SetNetwork(v string)`

SetNetwork sets Network field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


