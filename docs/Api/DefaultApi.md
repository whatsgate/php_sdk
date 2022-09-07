# Swagger\Client\DefaultApi

All URIs are relative to *https://whatsgate.ru/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**checkPost**](DefaultApi.md#checkpost) | **POST** /check | Проверка зарегистрирован ли номер в WhatsApp
[**getChatsPost**](DefaultApi.md#getchatspost) | **POST** /get-chats | Возвращает список активных чатов
[**seenPost**](DefaultApi.md#seenpost) | **POST** /seen | Отправляет команду в чат, что последние сообщения просмотрены
[**sendMessage**](DefaultApi.md#sendmessage) | **POST** /send | Отправка сообщения

# **checkPost**
> \Swagger\Client\Model\InlineResponse2001 checkPost($body)

Проверка зарегистрирован ли номер в WhatsApp

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: ApiKeyAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-API-Key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-API-Key', 'Bearer');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\CheckBody(); // \Swagger\Client\Model\CheckBody | Проверяет, зарегистрирован ли указанный номер в WhatsApp. Номер указывается в формате только цифр, например 79999999999

try {
    $result = $apiInstance->checkPost($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->checkPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\CheckBody**](../Model/CheckBody.md)| Проверяет, зарегистрирован ли указанный номер в WhatsApp. Номер указывается в формате только цифр, например 79999999999 |

### Return type

[**\Swagger\Client\Model\InlineResponse2001**](../Model/InlineResponse2001.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getChatsPost**
> \Swagger\Client\Model\InlineResponse2002 getChatsPost($body)

Возвращает список активных чатов

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: ApiKeyAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-API-Key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-API-Key', 'Bearer');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\GetchatsBody(); // \Swagger\Client\Model\GetchatsBody | Запрашивает и возвращает список активных чатов, включая контакты и группы. В объекте группы находится идентификатор группы, список всех участников группы, права участников (является ли участник администратором группы).

try {
    $result = $apiInstance->getChatsPost($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->getChatsPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\GetchatsBody**](../Model/GetchatsBody.md)| Запрашивает и возвращает список активных чатов, включая контакты и группы. В объекте группы находится идентификатор группы, список всех участников группы, права участников (является ли участник администратором группы). |

### Return type

[**\Swagger\Client\Model\InlineResponse2002**](../Model/InlineResponse2002.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **seenPost**
> \Swagger\Client\Model\InlineResponse2004 seenPost($body)

Отправляет команду в чат, что последние сообщения просмотрены

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: ApiKeyAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-API-Key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-API-Key', 'Bearer');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\SeenBody(); // \Swagger\Client\Model\SeenBody | Команда устанавливает у всех сообщений в указанном чате статус просмотрены.

try {
    $result = $apiInstance->seenPost($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->seenPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\SeenBody**](../Model/SeenBody.md)| Команда устанавливает у всех сообщений в указанном чате статус просмотрены. |

### Return type

[**\Swagger\Client\Model\InlineResponse2004**](../Model/InlineResponse2004.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sendMessage**
> \Swagger\Client\Model\InlineResponse200 sendMessage($body)

Отправка сообщения

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: ApiKeyAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-API-Key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-API-Key', 'Bearer');

$apiInstance = new Swagger\Client\Api\DefaultApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$body = new \Swagger\Client\Model\SendBody(); // \Swagger\Client\Model\SendBody | Отправляет текстовое или мультимедийное сообщение контакту либо группе. Может использоваться синхронно (возвращает ответ после отправки сообщения, ответ содержит объект отправленного сообщения с идентификатором), либо асинхронно (ответ содержит результат постановки в очередь, а отправленное сообщение приходит на указанный webhook). По умолчанию используется асинхронная отправка.

try {
    $result = $apiInstance->sendMessage($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sendMessage: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\SendBody**](../Model/SendBody.md)| Отправляет текстовое или мультимедийное сообщение контакту либо группе. Может использоваться синхронно (возвращает ответ после отправки сообщения, ответ содержит объект отправленного сообщения с идентификатором), либо асинхронно (ответ содержит результат постановки в очередь, а отправленное сообщение приходит на указанный webhook). По умолчанию используется асинхронная отправка. |

### Return type

[**\Swagger\Client\Model\InlineResponse200**](../Model/InlineResponse200.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

