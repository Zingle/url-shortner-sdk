# ZingleApi\UrlShortner\V1Api

All URIs are relative to *http://127.0.0.1:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**replace**](V1Api.md#replace) | **POST** /v1/replace | 
[**shorten**](V1Api.md#shorten) | **POST** /v1 | 
[**shortenBulk**](V1Api.md#shortenBulk) | **POST** /v1/bulk | 


# **replace**
> \ZingleApi\UrlShortner\Model\ReplacedText replace($replace_request)



Replace targetUrls in string

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


$apiInstance = new ZingleApi\UrlShortner\Api\V1Api(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$replace_request = new \ZingleApi\UrlShortner\Model\ReplaceRequest(); // \ZingleApi\UrlShortner\Model\ReplaceRequest | 

try {
    $result = $apiInstance->replace($replace_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling V1Api->replace: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **replace_request** | [**\ZingleApi\UrlShortner\Model\ReplaceRequest**](../Model/ReplaceRequest.md)|  | [optional]

### Return type

[**\ZingleApi\UrlShortner\Model\ReplacedText**](../Model/ReplacedText.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

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
> \ZingleApi\UrlShortner\Model\ShortUrl[] shortenBulk($bulk_shorten_request)



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
$bulk_shorten_request = new \ZingleApi\UrlShortner\Model\BulkShortenRequest(); // \ZingleApi\UrlShortner\Model\BulkShortenRequest | 

try {
    $result = $apiInstance->shortenBulk($bulk_shorten_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling V1Api->shortenBulk: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulk_shorten_request** | [**\ZingleApi\UrlShortner\Model\BulkShortenRequest**](../Model/BulkShortenRequest.md)|  | [optional]

### Return type

[**\ZingleApi\UrlShortner\Model\ShortUrl[]**](../Model/ShortUrl.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

