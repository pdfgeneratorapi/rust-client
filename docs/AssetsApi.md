# \AssetsApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generate_qr_code**](AssetsApi.md#generate_qr_code) | **POST** /assets/qrcode | Generate QR Code



## generate_qr_code

> std::path::PathBuf generate_qr_code(generate_qr_code_request)
Generate QR Code

Creates a QR code based on the configuration

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**generate_qr_code_request** | [**GenerateQrCodeRequest**](GenerateQrCodeRequest.md) | QR Code configuration | [required] |

### Return type

[**std::path::PathBuf**](std::path::PathBuf.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: image/png, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

