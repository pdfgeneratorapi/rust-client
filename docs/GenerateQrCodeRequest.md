# GenerateQrCodeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**content** | **String** | The content which is used to generate QR code | 
**color** | Option<**String**> | QR code color as a hex color code | [optional][default to #000000]
**logo_base64** | Option<**String**> | A logo as a base64 image string to add on the QR code. Cannot be combined with `logo_url`. | [optional]
**logo_url** | Option<**String**> | Public HTTPS URL of a logo image to add on the QR code. Cannot be combined with `logo_base64`. | [optional]
**output** | Option<**String**> | Response format | [optional][default to Base64]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


