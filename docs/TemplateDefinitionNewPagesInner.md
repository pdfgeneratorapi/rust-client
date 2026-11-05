# TemplateDefinitionNewPagesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**width** | Option<**f64**> | Page width in units | [optional]
**height** | Option<**f64**> | Page height in units | [optional]
**margins** | Option<[**models::TemplateDefinitionNewPagesInnerMargins**](TemplateDefinitionNew_pages_inner_margins.md)> |  | [optional]
**border** | Option<**bool**> | Stored for older templates. It draws nothing. | [optional][default to false]
**components** | Option<[**Vec<serde_json::Value>**](serde_json::Value.md)> | The page's components. The fields of each depend on its cls; the template schema (Get schema endpoint) lists them. | [optional]
**layout** | Option<[**models::TemplateDefinitionNewPagesInnerLayout**](TemplateDefinitionNew_pages_inner_layout.md)> |  | [optional]
**conditional_formats** | Option<[**Vec<serde_json::Value>**](serde_json::Value.md)> |  | [optional]
**background_image** | Option<**String**> | Defines background image for the page. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


