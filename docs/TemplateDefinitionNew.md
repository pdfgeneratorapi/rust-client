# TemplateDefinitionNew

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **String** | Template name | 
**tags** | Option<**Vec<String>**> | A list of tags assigned to a template | [optional]
**is_draft** | Option<**bool**> | Indicates if the template is a draft or published. | [optional]
**layout** | Option<[**models::TemplateDefinitionNewLayout**](TemplateDefinitionNew_layout.md)> |  | [optional]
**pages** | Option<[**Vec<models::TemplateDefinitionNewPagesInner>**](TemplateDefinitionNew_pages_inner.md)> | Defines page or label size, margins and components on page or label | [optional]
**data_settings** | Option<[**models::TemplateDefinitionNewDataSettings**](TemplateDefinitionNew_dataSettings.md)> |  | [optional]
**editor** | Option<[**models::TemplateDefinitionNewEditor**](TemplateDefinitionNew_editor.md)> |  | [optional]
**font_subsetting** | Option<**bool**> | If font-subsetting is applied to document when generated | [optional][default to false]
**barcode_as_image** | Option<**bool**> | Defines if barcodes are rendered as raster images instead of vector graphics. | [optional][default to false]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


