# EnableLogExportRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AuthPrincipal** | Pointer to **string** |  | [optional] 
**AwsExternalId** | Pointer to **string** | aws_external_id to include when assuming the IAM role specified by role_arn. Optional. A specific value may be required by the role&#39;s trust policy. Only supported for Advanced clusters on AWS. If provided for a Standard cluster, the request is rejected. | [optional] 
**AzureClientId** | Pointer to **string** | Azure client ID for the app registration used by the Logs Ingestion API. | [optional] 
**AzureClientSecret** | Pointer to **string** | Azure client secret for the app registration used by the Logs Ingestion API. | [optional] 
**AzureDceEndpoint** | Pointer to **string** | Logs ingestion endpoint of the Azure Data Collection Endpoint (DCE). | [optional] 
**AzureDcrImmutableId** | Pointer to **string** | Immutable ID of the Azure Data Collection Rule (DCR), for example dcr-... | [optional] 
**AzureDcrResourceId** | Pointer to **string** | Full ARM resource ID of the Azure Data Collection Rule (DCR). Cockroach Cloud reads and updates this DCR to add streams for each configured log group. | [optional] 
**AzureSharedKey** | Pointer to **string** | The primary or the secondary connected sources client authentication key. This is used to export logs to Azure Log Analytics via the legacy HTTP Data Collector API. Deprecated: use azure_client_secret instead. | [optional] 
**AzureTenantId** | Pointer to **string** | Azure tenant ID for the app registration used by the Logs Ingestion API. | [optional] 
**AzureWorkspaceResourceId** | Pointer to **string** | Full ARM resource ID of the Log Analytics workspace. Cockroach Cloud creates or updates the required custom tables for each configured log group. | [optional] 
**Groups** | Pointer to [**[]LogExportGroup**](LogExportGroup.md) | groups is a collection of log group configurations that allows the customer to define collections of CRDB log channels that are aggregated separately at the target sink. | [optional] 
**LogName** | **string** | log_name is an identifier for the logs in the customer&#39;s log sink. | 
**OmittedChannels** | Pointer to **[]string** | omitted_channels is a list of channels that the user does not want to export logs for. | [optional] 
**Redact** | Pointer to **bool** | redact allows the customer to set a default redaction policy for logs before they are exported to the target sink. If a group config omits a redact flag and this one is set to &#x60;true&#x60;, then that group will receive redacted logs. | [optional] 
**Region** | Pointer to **string** | region allows the customer to override the destination region for all logs for a cluster. | [optional] 
**Type** | [**LogExportType**](LogExportType.md) |  | 

## Methods

### NewEnableLogExportRequest

`func NewEnableLogExportRequest(logName string, type_ LogExportType, ) *EnableLogExportRequest`

NewEnableLogExportRequest instantiates a new EnableLogExportRequest object.
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed.

### NewEnableLogExportRequestWithDefaults

`func NewEnableLogExportRequestWithDefaults() *EnableLogExportRequest`

NewEnableLogExportRequestWithDefaults instantiates a new EnableLogExportRequest object.
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set.

### GetAuthPrincipal

`func (o *EnableLogExportRequest) GetAuthPrincipal() string`

GetAuthPrincipal returns the AuthPrincipal field if non-nil, zero value otherwise.

### SetAuthPrincipal

`func (o *EnableLogExportRequest) SetAuthPrincipal(v string)`

SetAuthPrincipal sets AuthPrincipal field to given value.

### GetAwsExternalId

`func (o *EnableLogExportRequest) GetAwsExternalId() string`

GetAwsExternalId returns the AwsExternalId field if non-nil, zero value otherwise.

### SetAwsExternalId

`func (o *EnableLogExportRequest) SetAwsExternalId(v string)`

SetAwsExternalId sets AwsExternalId field to given value.

### GetAzureClientId

`func (o *EnableLogExportRequest) GetAzureClientId() string`

GetAzureClientId returns the AzureClientId field if non-nil, zero value otherwise.

### SetAzureClientId

`func (o *EnableLogExportRequest) SetAzureClientId(v string)`

SetAzureClientId sets AzureClientId field to given value.

### GetAzureClientSecret

`func (o *EnableLogExportRequest) GetAzureClientSecret() string`

GetAzureClientSecret returns the AzureClientSecret field if non-nil, zero value otherwise.

### SetAzureClientSecret

`func (o *EnableLogExportRequest) SetAzureClientSecret(v string)`

SetAzureClientSecret sets AzureClientSecret field to given value.

### GetAzureDceEndpoint

`func (o *EnableLogExportRequest) GetAzureDceEndpoint() string`

GetAzureDceEndpoint returns the AzureDceEndpoint field if non-nil, zero value otherwise.

### SetAzureDceEndpoint

`func (o *EnableLogExportRequest) SetAzureDceEndpoint(v string)`

SetAzureDceEndpoint sets AzureDceEndpoint field to given value.

### GetAzureDcrImmutableId

`func (o *EnableLogExportRequest) GetAzureDcrImmutableId() string`

GetAzureDcrImmutableId returns the AzureDcrImmutableId field if non-nil, zero value otherwise.

### SetAzureDcrImmutableId

`func (o *EnableLogExportRequest) SetAzureDcrImmutableId(v string)`

SetAzureDcrImmutableId sets AzureDcrImmutableId field to given value.

### GetAzureDcrResourceId

`func (o *EnableLogExportRequest) GetAzureDcrResourceId() string`

GetAzureDcrResourceId returns the AzureDcrResourceId field if non-nil, zero value otherwise.

### SetAzureDcrResourceId

`func (o *EnableLogExportRequest) SetAzureDcrResourceId(v string)`

SetAzureDcrResourceId sets AzureDcrResourceId field to given value.

### GetAzureSharedKey

`func (o *EnableLogExportRequest) GetAzureSharedKey() string`

GetAzureSharedKey returns the AzureSharedKey field if non-nil, zero value otherwise.

### SetAzureSharedKey

`func (o *EnableLogExportRequest) SetAzureSharedKey(v string)`

SetAzureSharedKey sets AzureSharedKey field to given value.

### GetAzureTenantId

`func (o *EnableLogExportRequest) GetAzureTenantId() string`

GetAzureTenantId returns the AzureTenantId field if non-nil, zero value otherwise.

### SetAzureTenantId

`func (o *EnableLogExportRequest) SetAzureTenantId(v string)`

SetAzureTenantId sets AzureTenantId field to given value.

### GetAzureWorkspaceResourceId

`func (o *EnableLogExportRequest) GetAzureWorkspaceResourceId() string`

GetAzureWorkspaceResourceId returns the AzureWorkspaceResourceId field if non-nil, zero value otherwise.

### SetAzureWorkspaceResourceId

`func (o *EnableLogExportRequest) SetAzureWorkspaceResourceId(v string)`

SetAzureWorkspaceResourceId sets AzureWorkspaceResourceId field to given value.

### GetGroups

`func (o *EnableLogExportRequest) GetGroups() []LogExportGroup`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### SetGroups

`func (o *EnableLogExportRequest) SetGroups(v []LogExportGroup)`

SetGroups sets Groups field to given value.

### GetLogName

`func (o *EnableLogExportRequest) GetLogName() string`

GetLogName returns the LogName field if non-nil, zero value otherwise.

### SetLogName

`func (o *EnableLogExportRequest) SetLogName(v string)`

SetLogName sets LogName field to given value.

### GetOmittedChannels

`func (o *EnableLogExportRequest) GetOmittedChannels() []string`

GetOmittedChannels returns the OmittedChannels field if non-nil, zero value otherwise.

### SetOmittedChannels

`func (o *EnableLogExportRequest) SetOmittedChannels(v []string)`

SetOmittedChannels sets OmittedChannels field to given value.

### GetRedact

`func (o *EnableLogExportRequest) GetRedact() bool`

GetRedact returns the Redact field if non-nil, zero value otherwise.

### SetRedact

`func (o *EnableLogExportRequest) SetRedact(v bool)`

SetRedact sets Redact field to given value.

### GetRegion

`func (o *EnableLogExportRequest) GetRegion() string`

GetRegion returns the Region field if non-nil, zero value otherwise.

### SetRegion

`func (o *EnableLogExportRequest) SetRegion(v string)`

SetRegion sets Region field to given value.

### GetType

`func (o *EnableLogExportRequest) GetType() LogExportType`

GetType returns the Type field if non-nil, zero value otherwise.

### SetType

`func (o *EnableLogExportRequest) SetType(v LogExportType)`

SetType sets Type field to given value.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


