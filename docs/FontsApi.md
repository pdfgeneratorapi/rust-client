# \FontsApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_fonts**](FontsApi.md#get_fonts) | **GET** /fonts | Get fonts



## get_fonts

> models::GetFonts200Response get_fonts(covers)
Get fonts

Returns the fonts the workspace's templates can use, sorted by name. Use a font's `id` as a component's `fontFamily`; a font that is not in this list is drawn with Open Sans.  Each font lists the styles it has glyphs of its own for, and the Unicode blocks it has at least half of the characters of, with the share in percent. To check particular characters, pass them in `covers`. 

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**covers** | Option<**String**> | Text whose every character a font must have a glyph for, in its regular style, to be returned. Control characters are ignored. |  |

### Return type

[**models::GetFonts200Response**](getFonts_200_response.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

