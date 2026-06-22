# \ConversionApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**convert_html2_pdf**](ConversionApi.md#convert_html2_pdf) | **POST** /conversion/html2pdf | HTML to PDF
[**convert_pdf2_image**](ConversionApi.md#convert_pdf2_image) | **POST** /conversion/pdf2image | PDF to Image
[**convert_url2_pdf**](ConversionApi.md#convert_url2_pdf) | **POST** /conversion/url2pdf | URL to PDF



## convert_html2_pdf

> models::InlineObject9 convert_html2_pdf(convert_html2_pdf_request)
HTML to PDF

Converts HTML content to PDF

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**convert_html2_pdf_request** | [**ConvertHtml2PdfRequest**](ConvertHtml2PdfRequest.md) |  | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## convert_pdf2_image

> models::InlineObject10 convert_pdf2_image(convert_pdf2_image_request)
PDF to Image

Converts PDF document to images. Provide either a base64 encoded PDF or a public URL to a PDF file.

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**convert_pdf2_image_request** | [**ConvertPdf2ImageRequest**](ConvertPdf2ImageRequest.md) |  | [required] |

### Return type

[**models::InlineObject10**](inline_object_10.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## convert_url2_pdf

> models::InlineObject9 convert_url2_pdf(convert_url2_pdf_request)
URL to PDF

Converts public URL to PDF

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**convert_url2_pdf_request** | [**ConvertUrl2PdfRequest**](ConvertUrl2PdfRequest.md) |  | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

