# LogExportStatus

## Enum
> LogExportStatus encodes the possible states that a configuration can be in as it is created, deployed, and disabled.   - DELIVERY_ERROR: DELIVERY_ERROR indicates the export pipeline is enabled and running, but the destination is rejecting or failing to receive log records (observed via the collector's send-failure self-telemetry). The cause is intentionally not distinguished here — it may be invalid credentials, a wrong endpoint, or a transient outage at the destination — so user-facing messaging stays neutral.

* `DISABLED` (value: `"DISABLED"`)

* `DISABLING` (value: `"DISABLING"`)

* `DISABLE_FAILED` (value: `"DISABLE_FAILED"`)

* `ENABLED` (value: `"ENABLED"`)

* `ENABLING` (value: `"ENABLING"`)

* `ENABLE_FAILED` (value: `"ENABLE_FAILED"`)

* `CREDENTIALS_ERROR` (value: `"CREDENTIALS_ERROR"`)

* `DELIVERY_ERROR` (value: `"DELIVERY_ERROR"`)


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


