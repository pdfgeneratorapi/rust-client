# \EInvoicesApi

All URIs are relative to *https://us1.pdfgeneratorapi.com/api/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_e_invoice**](EInvoicesApi.md#create_e_invoice) | **POST** /einvoice | Create eInvoice
[**create_factur_xe_invoice**](EInvoicesApi.md#create_factur_xe_invoice) | **POST** /einvoice/facturx | Create Factur-X eInvoice
[**create_x_rechnung_e_invoice**](EInvoicesApi.md#create_x_rechnung_e_invoice) | **POST** /einvoice/xrechnung | Create XRechnung eInvoice
[**get_e_invoice_schema**](EInvoicesApi.md#get_e_invoice_schema) | **GET** /einvoice/schema | Get schema



## create_e_invoice

> models::InlineObject create_e_invoice(create_e_invoice_request)
Create eInvoice

This endpoint transforms a JSON payload into an XML-based e-invoice that is fully compliant with the European EN 16931 standard. The generated output can be formatted in either UBL (Universal Business Language) or CII (Cross-Industry Invoice) syntax, ensuring interoperability across B2B and B2G platforms. The JSON payload follows Peppol BIS Billing 3.0 UBL Invoice described here: https://docs.peppol.eu/poacc/billing/3.0/

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_e_invoice_request** | [**CreateEInvoiceRequest**](CreateEInvoiceRequest.md) | eInvoice conversion | [required] |

### Return type

[**models::InlineObject**](inline_object.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_factur_xe_invoice

> models::InlineObject9 create_factur_xe_invoice(create_factur_xe_invoice_request)
Create Factur-X eInvoice

This endpoint transforms a JSON payload a Factur-X e-invoice that is fully compliant with the European EN 16931 standard. The generated output is always a PDF document, embedding a structured CII (Cross-Industry Invoice) XML according to the Factur-X format into a human-readable invoice, ensuring interoperability across B2B and B2G platforms. The JSON payload follows Peppol BIS Billing 3.0 UBL Invoice described here: https://docs.peppol.eu/poacc/billing/3.0/

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_factur_xe_invoice_request** | [**CreateFacturXeInvoiceRequest**](CreateFacturXeInvoiceRequest.md) | eInvoice conversion | [required] |

### Return type

[**models::InlineObject9**](inline_object_9.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## create_x_rechnung_e_invoice

> models::InlineObject create_x_rechnung_e_invoice(create_e_invoice_request)
Create XRechnung eInvoice

This endpoint transforms a JSON payload into an XML-based XRechnung e-invoice that is fully compliant with the European EN 16931 standard. The generated output follows the XRechnung format and can be formatted in either UBL (Universal Business Language) or CII (Cross-Industry Invoice) syntax, ensuring interoperability across B2B and B2G platforms. The JSON payload follows Peppol BIS Billing 3.0 UBL Invoice described here: https://docs.peppol.eu/poacc/billing/3.0/

### Parameters


Name | Type | Description  | Required | Notes
------------- | ------------- | ------------- | ------------- | -------------
**create_e_invoice_request** | [**CreateEInvoiceRequest**](CreateEInvoiceRequest.md) | eInvoice conversion | [required] |

### Return type

[**models::InlineObject**](inline_object.md)

### Authorization

[JSONWebTokenAuth](../README.md#JSONWebTokenAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)


## get_e_invoice_schema

> serde_json::Value get_e_invoice_schema()
Get schema

Returns e-invoice JSON schema which defines the structure of the e-invoice.

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

