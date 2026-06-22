# ConvertPdf2ImageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_base64** | Option<**String**> | Base64 encoded PDF file. Required if file_url is not provided. | [optional]
**file_url** | Option<**String**> | Public HTTPS URL to a PDF file. Required if file_base64 is not provided. | [optional]
**format** | Option<**String**> | Output image format | [optional][default to Png]
**quality** | Option<**i32**> | Image quality (1-100) | [optional][default to 85]
**resolution** | Option<**i32**> | Image resolution in DPI (72-600) | [optional][default to 150]
**pages** | Option<**String**> | Page number or range to convert. Use a single number (e.g. \"1\") or a range (e.g. \"1-4\"). Defaults to all pages. | [optional][default to all]
**output** | Option<**String**> | Output format | [optional][default to Base64]
**name** | Option<**String**> | Document name (max 120 characters). Auto-generated if not provided. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


