# \DocumentsApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_document**](DocumentsApi.md#delete_document) | **DELETE** /documents/{publicId} | Delete document
[**generate_document**](DocumentsApi.md#generate_document) | **POST** /documents/generate | Generate document
[**generate_document_asynchronous**](DocumentsApi.md#generate_document_asynchronous) | **POST** /documents/generate/async | Generate document (async)
[**generate_document_batch**](DocumentsApi.md#generate_document_batch) | **POST** /documents/generate/batch | Generate document (batch)
[**generate_document_batch_asynchronous**](DocumentsApi.md#generate_document_batch_asynchronous) | **POST** /documents/generate/batch/async | Generate document (batch + async)
[**get_async_job_status**](DocumentsApi.md#get_async_job_status) | **GET** /documents/async/{jobId} | Get job status
[**get_document**](DocumentsApi.md#get_document) | **GET** /documents/{publicId} | Get document
[**get_documents**](DocumentsApi.md#get_documents) | **GET** /documents | Get documents
[**store_document**](DocumentsApi.md#store_document) | **POST** /documents | Store document



## delete_document

> delete_document(public_id)
Delete document

Delete document from the Document Storage

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**public_id** | **String** | Resource public id | [required] |

### Return type

 (empty response body)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## generate_document

> models::InlineObject9 generate_document(generate_document_request)
Generate document

Merges template with data and returns base64 encoded document or a public URL to a document. NB! When the public URL option is used, the document is stored for 30 days and automatically deleted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**generate_document_request** | [**GenerateDocumentRequest**](GenerateDocumentRequest.md) | Request parameters, including template id, data and formats. | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## generate_document_asynchronous

> models::InlineObject20 generate_document_asynchronous(generate_document_asynchronous_request)
Generate document (async)

Merges template with data as asynchronous job and makes POST request to callback URL defined in the request. Request uses the same format as response of synchronous generation endpoint. The job id is also added to the callback request as header PDF-API-Job-Id  *Example response from callback URL:* ``` {   \"response\": \"https://us1.pdfgeneratorapi.com/share/12821/VBERi0xLjcKJeLjz9MKNyAwIG9i\",   \"meta\": {     \"name\": \"a2bd25b8921f3dc7a440fd7f427f90a4.pdf\",     \"display_name\": \"a2bd25b8921f3dc7a440fd7f427f90a4\",     \"encoding\": \"binary\",     \"content-type\": \"application/pdf\"   } } ``` 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**generate_document_asynchronous_request** | [**GenerateDocumentAsynchronousRequest**](GenerateDocumentAsynchronousRequest.md) | Request parameters, including template id, data and formats. | [required] |

### Return type

[**models::InlineObject20**](inline_object_20.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## generate_document_batch

> models::InlineObject9 generate_document_batch(generate_document_batch_request)
Generate document (batch)

Allows to merge multiple templates with data and returns base64 encoded document or public URL to a document. NB! When the public URL option is used, the document is stored for 30 days and automatically deleted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**generate_document_batch_request** | [**GenerateDocumentBatchRequest**](GenerateDocumentBatchRequest.md) | Request parameters, including template id, data and formats. | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## generate_document_batch_asynchronous

> models::InlineObject20 generate_document_batch_asynchronous(generate_document_batch_asynchronous_request)
Generate document (batch + async)

Merges template with data as asynchronous job and makes POST request to callback URL defined in the request. Request uses the same format as response of synchronous generation endpoint. The job id is also added to the callback request as header PDF-API-Job-Id  *Example response from callback URL:* ``` {   \"response\": \"https://us1.pdfgeneratorapi.com/share/12821/VBERi0xLjcKJeLjz9MKNyAwIG9i\",   \"meta\": {     \"name\": \"a2bd25b8921f3dc7a440fd7f427f90a4.pdf\",     \"display_name\": \"a2bd25b8921f3dc7a440fd7f427f90a4\",     \"encoding\": \"binary\",     \"content-type\": \"application/pdf\"   } } ``` 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**generate_document_batch_asynchronous_request** | [**GenerateDocumentBatchAsynchronousRequest**](GenerateDocumentBatchAsynchronousRequest.md) | Request parameters, including template id, data and formats. | [required] |

### Return type

[**models::InlineObject20**](inline_object_20.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_async_job_status

> models::InlineObject13 get_async_job_status(job_id)
Get job status

Returns status of an async job

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**job_id** | **String** | Job id | [required] |

### Return type

[**models::InlineObject13**](inline_object_13.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_document

> models::InlineObject11 get_document(public_id)
Get document

Returns document stored in the Document Storage

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**public_id** | **String** | Resource public id | [required] |

### Return type

[**models::InlineObject11**](inline_object_11.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_documents

> models::InlineObject15 get_documents(template_id, start_date, end_date, page, per_page)
Get documents

Returns a list of generated documents created by authorized workspace and stored in PDF Generator API. If master user is specified as workspace in JWT then all documents created in the organization are returned. NB! This endpoint returns only documents generated using the output=url option.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | Option<**i32**> | Template unique identifier |  |
**start_date** | Option<**String**> | Start date. Format: Y-m-d H:i:s |  |
**end_date** | Option<**String**> | End date. Format: Y-m-d H:i:s. Defaults to current timestamp |  |
**page** | Option<**i32**> | Pagination: page to return |  |[default to 1]
**per_page** | Option<**i32**> | Pagination: How many records to return per page |  |[default to 15]

### Return type

[**models::InlineObject15**](inline_object_15.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## store_document

> models::InlineObject11 store_document(store_document_request)
Store document

Uploads a PDF as a URL or a base64 encoded string.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**store_document_request** | [**StoreDocumentRequest**](StoreDocumentRequest.md) | Document source and optional metadata. Exactly one of `file_base64` or `file_url` is required. | [required] |

### Return type

[**models::InlineObject11**](inline_object_11.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

