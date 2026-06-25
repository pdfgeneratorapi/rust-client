# \TemplateLibraryApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_template_library**](TemplateLibraryApi.md#get_template_library) | **GET** /templates/library | Get template library
[**get_template_library_item**](TemplateLibraryApi.md#get_template_library_item) | **GET** /templates/library/{publicId} | Open template from the library



## get_template_library

> models::GetTemplateLibrary200Response get_template_library(tags)
Get template library

Returns a list of publicly available templates from the template library. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**tags** | Option<**String**> | Filter template by tags |  |

### Return type

[**models::GetTemplateLibrary200Response**](getTemplateLibrary_200_response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_template_library_item

> models::InlineObject18 get_template_library_item(public_id)
Open template from the library

Returns the template definition for a public template identified by its `public_id`. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**public_id** | **String** | Resource public id | [required] |

### Return type

[**models::InlineObject18**](inline_object_18.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

