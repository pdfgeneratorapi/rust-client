# FormConfigurationNew

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**template_id** | Option<**i32**> | Template ID which is connected to the form | [optional]
**name** | **String** | Form name | 
**actions** | [**Vec<models::FormConfigurationNewActionsInner>**](FormConfigurationNew_actions_inner.md) | Array of action configurations. Each action is a separate object with a single key; leave an action out to disable it. | 
**fields** | [**Vec<models::FormField>**](formField.md) | Input fields shown on the form, in display order. Field names must be unique within the form. | 
**configuration** | Option<[**models::FormConfiguration**](formConfiguration.md)> |  | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


