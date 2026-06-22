# TemplateDefinition

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**i32**> | Unique identifier | [optional]
**name** | Option<**String**> | Template name | [optional]
**tags** | Option<**Vec<String>**> | A list of tags assigned to a template | [optional]
**is_draft** | Option<**bool**> | Indicates if the template is a draft or published. | [optional]
**layout** | Option<[**models::TemplateDefinitionNewLayout**](TemplateDefinitionNew_layout.md)> |  | [optional]
**pages** | Option<[**Vec<models::TemplateDefinitionPagesInner>**](TemplateDefinition_pages_inner.md)> | Defines page or label size, margins and components on page or label | [optional]
**data_settings** | Option<[**models::TemplateDefinitionDataSettings**](TemplateDefinition_dataSettings.md)> |  | [optional]
**editor** | Option<[**models::TemplateDefinitionEditor**](TemplateDefinition_editor.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


