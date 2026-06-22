# GenerateDocumentBatchAsynchronousRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template** | Option<[**Vec<models::TemplateParam>**](templateParam.md)> |  | [optional]
**callback** | Option<[**models::CallbackParam**](callbackParam.md)> |  | [optional]
**format** | Option<[**models::FormatParam**](formatParam.md)> |  | [optional]
**output** | Option<[**models::AsyncOutputParam**](asyncOutputParam.md)> |  | [optional]
**name** | Option<**String**> | Generated document name (optional) | [optional][default to ]
**testing** | Option<**bool**> | When set to true the generation is not counted as merge (monthly usage), but a large PREVIEW stamp is added. | [optional][default to false]
**metadata** | Option<[**models::MetadataParam**](metadataParam.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


