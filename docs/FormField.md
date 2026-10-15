# FormField

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **String** | Field label displayed in the form | 
**name** | **String** | Data field name. For example \"name\" can be used as \"{name}\" in the document as placeholder. | 
**r#type** | **String** | Field type * `text` - Free text input * `integer` - Whole number input * `number` - Decimal number input * `date` - Date picker * `signature` - Hand-drawn signature, stored as an image * `select` - Dropdown with a single choice. Requires `subRows` with options and a `default` value * `multi-select` - Dropdown with multiple choices. Requires `subRows` with options * `table` - Repeating rows of values. Its columns are defined in `subRows` * `image` - Image upload * `pdf` - PDF file upload  | 
**required** | **bool** | Specifies if the field is required or not | 
**default** | Option<**String**> | Value pre-filled in the field. Required for `select` fields and must be one of the options. Not used by `table` fields. | [optional]
**description** | Option<**String**> | Help text shown with the field | [optional]
**sub_rows** | Option<[**Vec<models::FormFieldSubRowsInner>**](formField_subRows_inner.md)> | Options for `select` and `multi-select` fields (a single object), columns for `table` fields. Not used by other field types. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


