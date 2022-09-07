# ResponseMessage

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Идентификатор сообщения | [optional] 
**ack** | **int** | Флаг просмотра сообщения | [optional] 
**has_media** | **bool** | Флаг, имеет ли сообщение медиафайл | [optional] 
**media_key** | **string** | Ключ медиафайла (при наличии) | [optional] 
**body** | **string** | Текст сообщения | [optional] 
**type** | **string** | Тип сообщения | [optional] 
**timestamp** | **int** | Время сообщения в формате Unix Timestamp | [optional] 
**from** | **string** | Идентификатор отправителя в формате WhatsApp | [optional] 
**to** | **string** | Идентификатор получателя в формате WhatsApp | [optional] 
**is_forwarded** | **bool** | Флаг, было ли сообщение перенаправлено | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

