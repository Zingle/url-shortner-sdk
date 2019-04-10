# ZingleApi\UrlShortner\V1Api

All URIs are relative to *http://127.0.0.1:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**shorten**](V1Api.md#shorten) | **POST** /v1 | 
[**shortenBulk**](V1Api.md#shortenBulk) | **POST** /v1/bulk | 


# **shorten**
> \ZingleApi\UrlShortner\Model\ShortUrl shorten($body)



Shorten a single URL

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


$apiInstance = new ZingleApi\UrlShortner\Api\V1Api(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \ZingleApi\UrlShortner\Model\ShortenRequest(); // \ZingleApi\UrlShortner\Model\ShortenRequest | 

try {
    $result = $apiInstance->shorten($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling V1Api->shorten: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **\ZingleApi\UrlShortner\Model\ShortenRequest**|  | [optional]

### Return type

[**\ZingleApi\UrlShortner\Model\ShortUrl**](../Model/ShortUrl.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **shortenBulk**
> \ZingleApi\UrlShortner\Model\ShortUrl[] shortenBulk($body)



Shorten a bulk URLs

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


$apiInstance = new ZingleApi\UrlShortner\Api\V1Api(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \ZingleApi\UrlShortner\Model\BulkShortenRequest(); // \ZingleApi\UrlShortner\Model\BulkShortenRequest | 

try {
    $result = $apiInstance->shortenBulk($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling V1Api->shortenBulk: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **\ZingleApi\UrlShortner\Model\BulkShortenRequest**|  | [optional]

### Return type

[**\ZingleApi\UrlShortner\Model\ShortUrl[]**](../Model/ShortUrl.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

