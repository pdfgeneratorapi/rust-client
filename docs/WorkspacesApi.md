# \WorkspacesApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_workspace**](WorkspacesApi.md#create_workspace) | **POST** /workspaces | Create workspace
[**delete_workspace**](WorkspacesApi.md#delete_workspace) | **DELETE** /workspaces/{workspaceIdentifier} | Delete workspace
[**get_workspace**](WorkspacesApi.md#get_workspace) | **GET** /workspaces/{workspaceIdentifier} | Get workspace
[**get_workspaces**](WorkspacesApi.md#get_workspaces) | **GET** /workspaces | Get workspaces



## create_workspace

> models::InlineObject7 create_workspace(create_workspace_request)
Create workspace

Creates a regular workspace with identifier specified in the request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_workspace_request** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md) |  | [required] |

### Return type

[**models::InlineObject7**](inline_object_7.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## delete_workspace

> delete_workspace(workspace_identifier)
Delete workspace

Delete workspace. Only regular workspaces can be deleted.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**workspace_identifier** | **String** | Workspace identifier | [required] |

### Return type

 (empty response body)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_workspace

> models::InlineObject7 get_workspace(workspace_identifier)
Get workspace

Returns workspace information for the workspace identifier specified in the request.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**workspace_identifier** | **String** | Workspace identifier | [required] |

### Return type

[**models::InlineObject7**](inline_object_7.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_workspaces

> models::InlineObject5 get_workspaces(page, per_page, order_by, order_direction, activated, search)
Get workspaces

Returns all workspaces in the organization

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**page** | Option<**i32**> | Pagination: page to return |  |[default to 1]
**per_page** | Option<**i32**> | Pagination: How many records to return per page |  |[default to 15]
**order_by** | Option<**String**> | Field to sort the workspaces by |  |[default to id]
**order_direction** | Option<**String**> | Sort direction |  |[default to desc]
**activated** | Option<**i32**> | Returns only active (`1`) or deactivated (`0`) workspaces |  |
**search** | Option<**String**> | Returns workspaces whose ID, name or identifier contains the search value |  |

### Return type

[**models::InlineObject5**](inline_object_5.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

