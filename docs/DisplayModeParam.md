# DisplayModeParam

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**zoom** | Option<**String**> | Initial zoom * `fullpage` - Fits the whole page in the window * `fullwidth` - Fits the page width to the window * `real` - Actual size (100%) * `default` - Leaves the zoom to the viewer. The PDF gets no open action, which some e-invoice validators require  | [optional][default to Fullwidth]
**layout** | Option<**String**> | Page layout * `SinglePage` - One page at a time * `OneColumn` - Pages in one continuous column * `TwoColumnLeft` - Pages in two columns, odd-numbered pages on the left * `TwoColumnRight` - Pages in two columns, odd-numbered pages on the right  | [optional][default to SinglePage]
**mode** | Option<**String**> | Panel shown when the document opens * `UseNone` - No panel * `UseOutlines` - Document outline (bookmarks) * `UseThumbs` - Page thumbnails * `FullScreen` - Full-screen mode, without menu bar or window controls  | [optional][default to UseNone]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


