# \TemplatesApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**copy_template**](TemplatesApi.md#copy_template) | **POST** /templates/{templateId}/copy | Copy template
[**create_template**](TemplatesApi.md#create_template) | **POST** /templates | Create template
[**delete_template**](TemplatesApi.md#delete_template) | **DELETE** /templates/{templateId} | Delete template
[**get_template**](TemplatesApi.md#get_template) | **GET** /templates/{templateId} | Get template
[**get_template_data**](TemplatesApi.md#get_template_data) | **GET** /templates/{templateId}/data | Get template data fields
[**get_template_schema**](TemplatesApi.md#get_template_schema) | **GET** /templates/schema | Get schema
[**get_templates**](TemplatesApi.md#get_templates) | **GET** /templates | Get templates
[**import_template**](TemplatesApi.md#import_template) | **POST** /templates/import | Import template
[**open_editor**](TemplatesApi.md#open_editor) | **POST** /templates/{templateId}/editor | Open editor
[**update_template**](TemplatesApi.md#update_template) | **PUT** /templates/{templateId} | Update template
[**validate_template**](TemplatesApi.md#validate_template) | **POST** /templates/validate | Validate template



## copy_template

> models::InlineObject16 copy_template(template_id, copy_template_request)
Copy template

Creates a copy of a template to the workspace specified in authentication parameters.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |
**copy_template_request** | Option<[**CopyTemplateRequest**](CopyTemplateRequest.md)> |  |  |

### Return type

[**models::InlineObject16**](inline_object_16.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_template

> models::InlineObject16 create_template(template_definition_new)
Create template

Creates a new template. If template configuration is not specified in the request body then an empty template is created. Template is placed to the workspace specified in authentication params. Template configuration must be sent in the request body.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_definition_new** | [**TemplateDefinitionNew**](TemplateDefinitionNew.md) | Template configuration | [required] |

### Return type

[**models::InlineObject16**](inline_object_16.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_template

> delete_template(template_id)
Delete template

Deletes the template from workspace

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |

### Return type

 (empty response body)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_template

> models::InlineObject16 get_template(template_id)
Get template

Returns template configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |

### Return type

[**models::InlineObject16**](inline_object_16.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_template_data

> models::InlineObject2 get_template_data(template_id)
Get template data fields

Returns all data fields used in the template. Returns structured JSON data that can be used to check which data fields are used in template or autogenerate sample data. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |

### Return type

[**models::InlineObject2**](inline_object_2.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_template_schema

> serde_json::Value get_template_schema()
Get schema

Returns Template JSON Schema which defines the structure of the Template Definition.

### Parameters

This endpoint does not need any parameter.

### Return type

[**serde_json::Value**](serde_json::Value.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_templates

> models::InlineObject4 get_templates(name, tags, access, page, per_page)
Get templates

Returns a list of templates available for the authenticated workspace

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**name** | Option<**String**> | Filter template by name |  |
**tags** | Option<**String**> | Filter template by tags |  |
**access** | Option<**String**> | Filter template by access type. No values returns all templates. private - returns only private templates, organization - returns only organization templates. |  |[default to ]
**page** | Option<**i32**> | Pagination: page to return |  |[default to 1]
**per_page** | Option<**i32**> | Pagination: How many records to return per page |  |[default to 15]

### Return type

[**models::InlineObject4**](inline_object_4.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## import_template

> models::InlineObject16 import_template(import_template_request)
Import template

Creates a template from existing PDF

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**import_template_request** | [**ImportTemplateRequest**](ImportTemplateRequest.md) | Import a PDF via URL or base64 string as template | [required] |

### Return type

[**models::InlineObject16**](inline_object_16.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## open_editor

> models::InlineObject3 open_editor(template_id, open_editor_request)
Open editor

Returns an unique URL which you can use to redirect your user to the editor from your application or use the generated URL as iframe source to show the editor within your application. When using iframe, make sure that your browser allows third-party cookies. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |
**open_editor_request** | [**OpenEditorRequest**](OpenEditorRequest.md) |  | [required] |

### Return type

[**models::InlineObject3**](inline_object_3.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_template

> models::InlineObject16 update_template(template_id, template_definition_new)
Update template

Updates template configuration. The template configuration for pages and layout must be complete as the entire configuration is replaced and not merged.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_id** | **i32** | Template unique identifier | [required] |
**template_definition_new** | [**TemplateDefinitionNew**](TemplateDefinitionNew.md) | Template configuration | [required] |

### Return type

[**models::InlineObject16**](inline_object_16.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## validate_template

> models::InlineObject1 validate_template(template_definition_new)
Validate template

Validates if the provided template configuration matches the template JSON schema.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**template_definition_new** | [**TemplateDefinitionNew**](TemplateDefinitionNew.md) | Template configuration | [required] |

### Return type

[**models::InlineObject1**](inline_object_1.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

