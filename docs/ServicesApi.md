# \ServicesApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_watermark**](ServicesApi.md#add_watermark) | **POST** /pdfservices/watermark | Add watermark
[**decrypt_document**](ServicesApi.md#decrypt_document) | **POST** /pdfservices/decrypt | Decrypt document
[**encrypt_document**](ServicesApi.md#encrypt_document) | **POST** /pdfservices/encrypt | Encrypt document
[**extract_form_fields**](ServicesApi.md#extract_form_fields) | **POST** /pdfservices/form/fields | Extract form fields
[**fill_form_fields**](ServicesApi.md#fill_form_fields) | **POST** /pdfservices/form/fill | Fill form fields
[**make_accessible**](ServicesApi.md#make_accessible) | **POST** /pdfservices/make-accessible | Make accessible
[**optimize_document**](ServicesApi.md#optimize_document) | **POST** /pdfservices/optimize | Optimize document



## add_watermark

> models::InlineObject9 add_watermark(add_watermark_request)
Add watermark

Adds a text or an image watermark to PDF document from base64 string or a remote URL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**add_watermark_request** | [**AddWatermarkRequest**](AddWatermarkRequest.md) |  | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## decrypt_document

> models::InlineObject9 decrypt_document(encrypt_document_request)
Decrypt document

Decrypts an encrypted PDF document from base64 string or a remote URL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**encrypt_document_request** | [**EncryptDocumentRequest**](EncryptDocumentRequest.md) |  | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## encrypt_document

> models::InlineObject9 encrypt_document(encrypt_document_request)
Encrypt document

Encrypts a PDF document from base64 string or a remote URL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**encrypt_document_request** | [**EncryptDocumentRequest**](EncryptDocumentRequest.md) |  | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## extract_form_fields

> models::InlineObject14 extract_form_fields(extract_form_fields_request)
Extract form fields

Extracts form fields and their metadata from a PDF document using base64 string or a remote URL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**extract_form_fields_request** | [**ExtractFormFieldsRequest**](ExtractFormFieldsRequest.md) |  | [required] |

### Return type

[**models::InlineObject14**](inline_object_14.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## fill_form_fields

> models::InlineObject9 fill_form_fields(fill_form_fields_request)
Fill form fields

Fills form fields in a PDF document with provided data from base64 string or a remote URL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**fill_form_fields_request** | [**FillFormFieldsRequest**](FillFormFieldsRequest.md) |  | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## make_accessible

> models::InlineObject9 make_accessible(make_accessible_request)
Make accessible

Tags a PDF document for accessibility from base64 string or a remote URL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**make_accessible_request** | [**MakeAccessibleRequest**](MakeAccessibleRequest.md) |  | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## optimize_document

> models::InlineObject12 optimize_document(optimize_document_request)
Optimize document

Optimizes the size of a PDF document from base64 string or a remote URL.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**optimize_document_request** | [**OptimizeDocumentRequest**](OptimizeDocumentRequest.md) |  | [required] |

### Return type

[**models::InlineObject12**](inline_object_12.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

