# \FormsApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_form**](FormsApi.md#create_form) | **POST** /forms | Create form
[**delete_form**](FormsApi.md#delete_form) | **DELETE** /forms/{formId} | Delete form
[**get_form**](FormsApi.md#get_form) | **GET** /forms/{formId} | Get form
[**get_forms**](FormsApi.md#get_forms) | **GET** /forms | Get forms
[**import_form**](FormsApi.md#import_form) | **POST** /forms/import | Import Form
[**open_form_builder**](FormsApi.md#open_form_builder) | **POST** /forms/open | Open new form builder
[**open_form_builder_for_existing_form**](FormsApi.md#open_form_builder_for_existing_form) | **POST** /forms/{formId}/open | Open existing form builder
[**share_form**](FormsApi.md#share_form) | **POST** /forms/{formId}/share | Share form
[**update_form**](FormsApi.md#update_form) | **PUT** /forms/{formId} | Update form



## create_form

> models::InlineObject17 create_form(form_configuration_new)
Create form

Creates a new form based on the configuration sent in the request body.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**form_configuration_new** | [**FormConfigurationNew**](FormConfigurationNew.md) | Form configuration | [required] |

### Return type

[**models::InlineObject17**](inline_object_17.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_form

> delete_form(form_id)
Delete form

Deletes the form with specified id

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**form_id** | **i32** | Form unique identifier | [required] |

### Return type

 (empty response body)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_form

> models::InlineObject17 get_form(form_id)
Get form

Returns form configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**form_id** | **i32** | Form unique identifier | [required] |

### Return type

[**models::InlineObject17**](inline_object_17.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_forms

> models::InlineObject6 get_forms(page, per_page)
Get forms

Returns a list of forms available for the organization

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**page** | Option<**i32**> | Pagination: page to return |  |[default to 1]
**per_page** | Option<**i32**> | Pagination: How many records to return per page |  |[default to 15]

### Return type

[**models::InlineObject6**](inline_object_6.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## import_form

> models::InlineObject17 import_form(import_form_request)
Import Form

Creates a new form based on editable PDF

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**import_form_request** | [**ImportFormRequest**](ImportFormRequest.md) | Import editable PDF via URL or base64 string as form | [required] |

### Return type

[**models::InlineObject17**](inline_object_17.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## open_form_builder

> models::InlineObject19 open_form_builder()
Open new form builder

Creates a new Form Builder session and returns a URL that can be used to open the embeddable Form Builder for creating a new form.

### Parameters

This endpoint does not need any parameter.

### Return type

[**models::InlineObject19**](inline_object_19.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## open_form_builder_for_existing_form

> models::InlineObject19 open_form_builder_for_existing_form(form_id)
Open existing form builder

Creates a Form Builder session for editing an existing form and returns a URL that can be used to open the embeddable Form Builder.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**form_id** | **i32** | Form unique identifier | [required] |

### Return type

[**models::InlineObject19**](inline_object_19.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## share_form

> models::InlineObject18 share_form(form_id)
Share form

Creates an unique sharing URL to collect form data

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**form_id** | **i32** | Form unique identifier | [required] |

### Return type

[**models::InlineObject18**](inline_object_18.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## update_form

> models::InlineObject17 update_form(form_id, form_configuration_new)
Update form

Updates the form configuration. The form configuration must be complete as the entire configuration is replaced and not merged.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**form_id** | **i32** | Form unique identifier | [required] |
**form_configuration_new** | [**FormConfigurationNew**](FormConfigurationNew.md) | Form configuration | [required] |

### Return type

[**models::InlineObject17**](inline_object_17.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

