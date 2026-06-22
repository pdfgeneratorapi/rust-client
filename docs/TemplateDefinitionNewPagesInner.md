# TemplateDefinitionNewPagesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**width** | Option<**f64**> | Page width in units | [optional]
**height** | Option<**f64**> | Page height in units | [optional]
**margins** | Option<[**models::TemplateDefinitionNewPagesInnerMargins**](TemplateDefinitionNew_pages_inner_margins.md)> |  | [optional]
**border** | Option<**bool**> |  | [optional][default to false]
**components** | Option<[**Vec<serde_json::Value>**](serde_json::Value.md)> |  | [optional]
**layout** | Option<[**serde_json::Value**](.md)> | Defines page specific layout which can differ from the main template layout (e.g page format, margins). | [optional]
**conditional_formats** | Option<[**Vec<serde_json::Value>**](serde_json::Value.md)> |  | [optional]
**background_image** | Option<**String**> | Defines background image for the page. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


