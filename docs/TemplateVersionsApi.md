# \TemplateVersionsApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_template_version**](TemplateVersionsApi.md#delete_template_version) | **DELETE** /templates/{templateId}/versions/{templateVersion} | Delete template version
[**get_template_version**](TemplateVersionsApi.md#get_template_version) | **GET** /templates/{templateId}/versions/{templateVersion} | Get template version
[**list_template_versions**](TemplateVersionsApi.md#list_template_versions) | **GET** /templates/{templateId}/versions | List template versions
[**promote_template_version**](TemplateVersionsApi.md#promote_template_version) | **PUT** /templates/{templateId}/versions/{templateVersion}/promote | Promote template version



## delete_template_version

> delete_template_version(template_id, template_version)
Delete template version

Deletes the specified template version. Production versions cannot be deleted. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |
**template_version** | **i32** | Unique ID of the template version. | [required] |

### Return type

 (empty response body)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_template_version

> models::InlineObject18 get_template_version(template_id, template_version)
Get template version

Returns the template definition of the specified version. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |
**template_version** | **i32** | Unique ID of the template version. | [required] |

### Return type

[**models::InlineObject18**](inline_object_18.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## list_template_versions

> models::TemplateVersionCollection list_template_versions(template_id, per_page, page)
List template versions

Returns a paginated list of template versions for the specified template. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |
**per_page** | Option<**i32**> | Number of items per page. |  |
**page** | Option<**i32**> | Page number to return. |  |

### Return type

[**models::TemplateVersionCollection**](TemplateVersionCollection.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## promote_template_version

> models::PromoteTemplateVersion200Response promote_template_version(template_id, template_version)
Promote template version

Promotes the specified template version to production. Only one version can be production at a time. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |
**template_version** | **i32** | Unique ID of the template version. | [required] |

### Return type

[**models::PromoteTemplateVersion200Response**](promoteTemplateVersion_200_response.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

