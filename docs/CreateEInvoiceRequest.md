# CreateEInvoiceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**serde_json::Value**](.md) | JSON payload that represents the Peppol BIS Billing 3.0 UBL Invoice (https://docs.peppol.eu/poacc/billing/3.0/) Use the Get schema endpoint to see the detailed payload structure. | 
**r#type** | Option<**String**> | Formatting type. | [optional][default to Ubl]
**output** | Option<**String**> | Response format. When the \"file\" option is used the API returns the file inline. | [optional][default to Base64]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


