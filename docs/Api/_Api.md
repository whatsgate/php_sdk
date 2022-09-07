# Swagger\Client\_Api

All URIs are relative to *https://whatsgate.ru/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getMediaPost**](_Api.md#getmediapost) | **POST** /get-media | Возвращает объект медиафайла, прикрепленного к сообщению

# **getMediaPost**
> \Swagger\Client\Model\InlineResponse2003 getMediaPost($body)

Возвращает объект медиафайла, прикрепленного к сообщению

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: ApiKeyAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-API-Key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-API-Key', 'Bearer');

$apiInstance = new Swagger\Client\Api\_Api(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\GetmediaBody(); // \Swagger\Client\Model\GetmediaBody | Запрашивает и возвращает медиа-файл, прикрепленный к сообщению по идентификатору mediaKey.

try {
    $result = $apiInstance->getMediaPost($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling _Api->getMediaPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\GetmediaBody**](../Model/GetmediaBody.md)| Запрашивает и возвращает медиа-файл, прикрепленный к сообщению по идентификатору mediaKey. |

### Return type

[**\Swagger\Client\Model\InlineResponse2003**](../Model/InlineResponse2003.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

