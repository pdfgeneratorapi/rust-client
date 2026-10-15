# FormTableColumn

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**label** | **String** | Column label displayed in the form | 
**name** | **String** | Data field name of the column | 
**r#type** | **String** | Column type. `select` columns require `subRows` with options and a `default` value. | 
**required** | **bool** | Specifies if the column is required or not | 
**default** | Option<**String**> | Value pre-filled in the column. Required for `select` columns and must be one of the options. | [optional]
**sub_rows** | Option<[**Vec<models::FormFieldOptions>**](formFieldOptions.md)> | Options for `select` columns (a single object). Not used by other column types. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


