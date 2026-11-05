# TemplateDefinitionNewLayout

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**format** | **String** | Defines template page size. For any other size, use custom with width and height. | 
**width** | Option<**f64**> | Page width in units. Left out, it is the format's width; send it with a custom format. | [optional]
**height** | Option<**f64**> | Page height in units. Left out, it is the format's height; send it with a custom format. | [optional]
**unit** | Option<**String**> | Measure unit | [optional][default to Cm]
**orientation** | **String** | Page orientation | 
**rotation** | Option<**i32**> | Page rotation in degrees | [optional]
**margins** | [**models::TemplateDefinitionNewLayoutMargins**](TemplateDefinitionNew_layout_margins.md) |  | 
**repeat_layout** | Option<[**models::TemplateDefinitionNewLayoutRepeatLayout**](TemplateDefinitionNew_layout_repeatLayout.md)> |  | [optional]
**empty_labels** | Option<**i32**> | Specifies how many blank lables to add to sheet label. | [optional][default to 0]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


