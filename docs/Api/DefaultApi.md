# ZingleApi\UrlShortner\DefaultApi

All URIs are relative to *http://127.0.0.1:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getHealthCheck**](DefaultApi.md#getHealthCheck) | **GET** /_internal_/health | 


# **getHealthCheck**
> getHealthCheck()



Checks health of service

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


$apiInstance = new ZingleApi\UrlShortner\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->getHealthCheck();
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getHealthCheck: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

