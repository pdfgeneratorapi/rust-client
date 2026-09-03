# DocumentSignatures

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | Option<**String**> | The one-line answer, reduced from every signature worst case first. `unavailable` means signature validation is not enabled on this deployment — it says nothing about the document.  | [optional]
**status_label** | Option<**String**> | The status in words, ready to display. | [optional]
**has_long_term_validation** | Option<**bool**> | The document carries the certificate and revocation data needed to verify it after the signing certificates expire.  | [optional]
**covers_whole_document** | Option<**bool**> | The last signature covers every byte, so nothing was appended after it. | [optional]
**document_timestamps** | Option<**i32**> | Timestamp-only signatures, counted rather than listed: they are machinery, not people, and would double every signer.  | [optional]
**signatures** | Option<[**Vec<models::DocumentSignature>**](DocumentSignature.md)> | One entry per signature, excluding document timestamps. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


