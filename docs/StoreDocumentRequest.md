# StoreDocumentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_base64** | Option<**String**> | Base64 encoded PDF file. Required if file_url is not provided. | [optional]
**file_url** | Option<**String**> | Public HTTPS URL to a PDF file. Required if file_base64 is not provided. | [optional]
**name** | Option<**String**> | Generated document name (optional) | [optional][default to ]
**output** | Option<**String**> | Response format. `url` returns a public URL to the stored document; `viewer` returns a public URL to the PDF viewer. | [optional][default to Url]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


