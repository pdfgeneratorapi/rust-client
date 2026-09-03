# DocumentSignature

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**field_name** | Option<**String**> | Name of the signature field in the document. | [optional]
**signer_name** | Option<**String**> | The name the signer signed under. | [optional]
**signer** | Option<**String**> | Subject of the certificate that sealed it — an organization, not a person. | [optional]
**issuer** | Option<**String**> | Subject of the certificate authority that issued it. | [optional]
**signed_at** | Option<**String**> | When a timestamp authority attested the signature (ISO-8601). This is the defensible time; the signer's own clock proves nothing.  | [optional]
**claimed_signed_at** | Option<**String**> | The time the signer's own software recorded (ISO-8601). | [optional]
**timestamp_authority** | Option<**String**> | The timestamp authority that attested the signature. | [optional]
**intact** | Option<**bool**> | The bytes this signature covers are unchanged. | [optional]
**valid** | Option<**bool**> | The signature block itself adds up. On its own this does NOT mean the document is unchanged: a tampered file reports `valid` true with `intact` false, so a verdict needs intact AND valid AND trusted.  | [optional]
**trusted** | Option<**bool**> | The certificate chains to a trusted root. | [optional]
**coverage** | Option<**String**> | How much of the file this signature protects. | [optional]
**ades_indication** | Option<**String**> | The ETSI EN 319 102-1 indication, when the AdES engine could run. | [optional]
**ades_sub_indication** | Option<**String**> | The AdES sub-indication, naming why an indication is not PASSED. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


