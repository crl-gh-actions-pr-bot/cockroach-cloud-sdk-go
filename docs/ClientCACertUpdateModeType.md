# ClientCACertUpdateModeType

## Enum
>  - REPLACE: REPLACE overwrites all existing certs with the provided cert. This matches the behavior of the SetClientCACert (POST) endpoint.  - APPEND: APPEND adds the provided cert to the existing cert bundle. This enables no-downtime certificate rotation: append the new cert, roll it out across clients, then REPLACE with only the new cert to drop the old one.

* `REPLACE` (value: `"REPLACE"`)

* `APPEND` (value: `"APPEND"`)


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


