# GenerateDocumentRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template** | Option<[**models::TemplateParam**](templateParam.md)> |  | [optional]
**format** | Option<[**models::FormatParam**](formatParam.md)> |  | [optional]
**output** | Option<[**models::OutputParam**](outputParam.md)> |  | [optional]
**name** | Option<**String**> | Generated document name (optional) | [optional][default to ]
**testing** | Option<**bool**> | When set to true the generation is not counted as merge (monthly usage), but a large PREVIEW stamp is added. | [optional][default to false]
**make_accessible** | Option<**bool**> | Enables semantic document tagging. When enabled, a separate Make Accessible action is executed, which consumes additional credits. | [optional][default to false]
**print** | Option<**bool**> | When set to true, the PDF opens the print dialog when it is opened in a viewer. | [optional][default to false]
**empty_labels** | Option<**i32**> | Number of label positions to leave empty at the start of the first sheet. Only applies to label templates. | [optional][default to 0]
**attachments** | Option<[**Vec<models::AttachmentsParamInner>**](attachmentsParam_inner.md)> | Files embedded into the generated PDF as attachments. Only PDF and XML files are accepted. | [optional]
**metadata** | Option<[**models::MetadataParam**](metadataParam.md)> |  | [optional]
**display_mode** | Option<[**models::DisplayModeParam**](displayModeParam.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


