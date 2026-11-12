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
**background_image** | Option<**String**> | The page's background image: an image URL, a data URI or a {data field} placeholder, PNG, JPEG, GIF or SVG. It is drawn over the background color and under everything else on the page, as backgroundImageFit says. A template with a background PDF does not draw it. Empty or null for none. | [optional]
**background_color** | Option<**String**> | The page's background color in hex color code, #RRGGBB or #RGB, or with an alpha, #RRGGBBAA, #RGBA or rgba(r, g, b, a); a translucent one is lighter, the white of the paper showing through. It fills every sheet the page runs onto, edge to edge, under everything on it, the background image included; on a sheet of labels it fills each label. A template with a background PDF is not filled. Empty or null for none. | [optional]
**background_image_fit** | Option<**String**> | How the background image covers the page, centred: `stretch`, stretched to the page, as when none is set; `contain`, fitted inside the page, keeping its proportions; `cover`, filling the page, keeping its proportions, with what overflows cut off. Null for stretch. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


