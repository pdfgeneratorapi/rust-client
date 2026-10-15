# ConvertUrl2PdfRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**url** | Option<**String**> | Public URL | [optional]
**paper_size** | Option<**String**> | PDF page size | [optional][default to A4]
**orientation** | Option<**String**> |  | [optional][default to Portrait]
**output** | Option<**String**> | Output | [optional][default to Base64]
**filename** | Option<**String**> | Document name | [optional]
**wait_for_css** | Option<**String**> | CSS selector of an element to wait for before the page is printed; see `wait_for_css_state` | [optional]
**wait_for_css_state** | Option<**String**> | How `wait_for_css` matches. `present` waits until the element exists, even if it is empty or hidden (e.g. a `<div id=\"report-ready\"></div>` marker); `visible` waits until it is also visible with a non-empty size (e.g. a chart that appears when data has loaded). | [optional][default to Present]
**wait_for_js** | Option<**String**> | JavaScript expression evaluated in the page every 100ms; the page is printed once it is truthy. Promises are awaited, and an expression that throws counts as not ready yet. | [optional]
**wait_timeout** | Option<**i32**> | Seconds to wait for `wait_for_css` / `wait_for_js` before applying `on_wait_timeout` | [optional][default to 30]
**on_wait_timeout** | Option<**String**> | What to do when the wait signal is not met within `wait_timeout`. `error` returns a 422 response; `print` prints the page as it is. | [optional][default to Error]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


