# \DefaultApi

All URIs are relative to *https://api.amber.com.au/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SitesGet**](DefaultApi.md#SitesGet) | **Get** /sites | 
[**SitesSiteIdPricesCurrentGet**](DefaultApi.md#SitesSiteIdPricesCurrentGet) | **Get** /sites/{siteId}/prices/current | 
[**SitesSiteIdPricesGet**](DefaultApi.md#SitesSiteIdPricesGet) | **Get** /sites/{siteId}/prices | 
[**SitesSiteIdUsageGet**](DefaultApi.md#SitesSiteIdUsageGet) | **Get** /sites/{siteId}/usage | 



## SitesGet

> []InlineResponse200 SitesGet(ctx).Execute()





### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DefaultApi.SitesGet(context.Background()).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DefaultApi.SitesGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `SitesGet`: []InlineResponse200
    fmt.Fprintf(os.Stdout, "Response from `DefaultApi.SitesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiSitesGetRequest struct via the builder pattern


### Return type

[**[]InlineResponse200**](InlineResponse200.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SitesSiteIdPricesCurrentGet

> []AnyOfAnyTypeAnyTypeAnyType SitesSiteIdPricesCurrentGet(ctx, siteId).Next(next).Previous(previous).Resolution(resolution).Execute()





### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    siteId := "siteId_example" // string | ID of the site you are fetching prices for. Can be found using the `/sites` enpoint
    next := float32(8.14) // float32 | Return the _next_ number of forecast intervals (optional) (default to 0)
    previous := float32(8.14) // float32 | Return the _previous_ number of actual intervals. (optional) (default to 0)
    resolution := float32(8.14) // float32 | Specify the required interval duration resolution. Valid options: 30. Default: 30 (optional) (default to 30)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DefaultApi.SitesSiteIdPricesCurrentGet(context.Background(), siteId).Next(next).Previous(previous).Resolution(resolution).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DefaultApi.SitesSiteIdPricesCurrentGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `SitesSiteIdPricesCurrentGet`: []AnyOfAnyTypeAnyTypeAnyType
    fmt.Fprintf(os.Stdout, "Response from `DefaultApi.SitesSiteIdPricesCurrentGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**siteId** | **string** | ID of the site you are fetching prices for. Can be found using the &#x60;/sites&#x60; enpoint | 

### Other Parameters

Other parameters are passed through a pointer to a apiSitesSiteIdPricesCurrentGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **next** | **float32** | Return the _next_ number of forecast intervals | [default to 0]
 **previous** | **float32** | Return the _previous_ number of actual intervals. | [default to 0]
 **resolution** | **float32** | Specify the required interval duration resolution. Valid options: 30. Default: 30 | [default to 30]

### Return type

[**[]AnyOfAnyTypeAnyTypeAnyType**](anyOf&lt;AnyType,AnyType,AnyType&gt;.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SitesSiteIdPricesGet

> []AnyOfAnyTypeAnyTypeAnyType SitesSiteIdPricesGet(ctx, siteId).StartDate(startDate).EndDate(endDate).Resolution(resolution).Execute()





### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    siteId := "siteId_example" // string | ID of the site you are fetching prices for. Can be found using the `/sites` endpoint
    startDate := TODO // interface{} | Return all prices for each interval on and after this day. Defaults to today. (optional)
    endDate := TODO // interface{} | Return all prices for each interval on and before this day. Defaults to today. (optional)
    resolution := float32(8.14) // float32 | Specify the required interval duration resolution. Valid options: 5, 30. Default: 30 (optional) (default to 30)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DefaultApi.SitesSiteIdPricesGet(context.Background(), siteId).StartDate(startDate).EndDate(endDate).Resolution(resolution).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DefaultApi.SitesSiteIdPricesGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `SitesSiteIdPricesGet`: []AnyOfAnyTypeAnyTypeAnyType
    fmt.Fprintf(os.Stdout, "Response from `DefaultApi.SitesSiteIdPricesGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**siteId** | **string** | ID of the site you are fetching prices for. Can be found using the &#x60;/sites&#x60; endpoint | 

### Other Parameters

Other parameters are passed through a pointer to a apiSitesSiteIdPricesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **startDate** | [**interface{}**](interface{}.md) | Return all prices for each interval on and after this day. Defaults to today. | 
 **endDate** | [**interface{}**](interface{}.md) | Return all prices for each interval on and before this day. Defaults to today. | 
 **resolution** | **float32** | Specify the required interval duration resolution. Valid options: 5, 30. Default: 30 | [default to 30]

### Return type

[**[]AnyOfAnyTypeAnyTypeAnyType**](anyOf&lt;AnyType,AnyType,AnyType&gt;.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SitesSiteIdUsageGet

> []interface{} SitesSiteIdUsageGet(ctx, siteId).StartDate(startDate).EndDate(endDate).Resolution(resolution).Execute()





### Example

```go
package main

import (
    "context"
    "fmt"
    "os"
    openapiclient "./openapi"
)

func main() {
    siteId := "siteId_example" // string | ID of the site you are fetching usage for. Can be found using the `/sites` enpoint
    startDate := TODO // interface{} | Return all usage for each interval on and after this day.
    endDate := TODO // interface{} | Return all usage for each interval on and before this day.
    resolution := float32(8.14) // float32 | Specify the required interval duration resolution. Valid options: 30. Default: 30 (optional) (default to 30)

    configuration := openapiclient.NewConfiguration()
    apiClient := openapiclient.NewAPIClient(configuration)
    resp, r, err := apiClient.DefaultApi.SitesSiteIdUsageGet(context.Background(), siteId).StartDate(startDate).EndDate(endDate).Resolution(resolution).Execute()
    if err != nil {
        fmt.Fprintf(os.Stderr, "Error when calling `DefaultApi.SitesSiteIdUsageGet``: %v\n", err)
        fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
    }
    // response from `SitesSiteIdUsageGet`: []interface{}
    fmt.Fprintf(os.Stdout, "Response from `DefaultApi.SitesSiteIdUsageGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**siteId** | **string** | ID of the site you are fetching usage for. Can be found using the &#x60;/sites&#x60; enpoint | 

### Other Parameters

Other parameters are passed through a pointer to a apiSitesSiteIdUsageGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **startDate** | [**interface{}**](interface{}.md) | Return all usage for each interval on and after this day. | 
 **endDate** | [**interface{}**](interface{}.md) | Return all usage for each interval on and before this day. | 
 **resolution** | **float32** | Specify the required interval duration resolution. Valid options: 30. Default: 30 | [default to 30]

### Return type

**[]interface{}**

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

