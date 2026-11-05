# Font

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** | The value of a component's `fontFamily` for this font | 
**name** | **String** | Font name, as the editor shows it | 
**parent** | Option<**String**> | The `id` of the font this one is grouped under, such as another weight of the same family | 
**styles** | **Vec<String>** | The styles the font has glyphs of its own for. Text in another style is drawn with the regular glyphs. | 
**blocks** | **std::collections::HashMap<String, i32>** | The Unicode blocks the font has at least half of the characters of, with the share it has in percent. 100 means every character of the block. | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


