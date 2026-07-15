# PatchUserRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Operations** | [**[]ScimOperations**](ScimOperations.md) |  | 
**Schemas** | **[]string** | A list of one or more URIs identifying SCIM schemas that define the structure of the attributes in the request. The only supported schema at this time is \&quot;urn:ietf:params:scim:api:messages:2.0:PatchOp\&quot;. | 

## Methods

### NewPatchUserRequest

`func NewPatchUserRequest(operations []ScimOperations, schemas []string, ) *PatchUserRequest`

NewPatchUserRequest instantiates a new PatchUserRequest object.
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed.

### NewPatchUserRequestWithDefaults

`func NewPatchUserRequestWithDefaults() *PatchUserRequest`

NewPatchUserRequestWithDefaults instantiates a new PatchUserRequest object.
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set.

### GetOperations

`func (o *PatchUserRequest) GetOperations() []ScimOperations`

GetOperations returns the Operations field if non-nil, zero value otherwise.

### SetOperations

`func (o *PatchUserRequest) SetOperations(v []ScimOperations)`

SetOperations sets Operations field to given value.

### GetSchemas

`func (o *PatchUserRequest) GetSchemas() []string`

GetSchemas returns the Schemas field if non-nil, zero value otherwise.

### SetSchemas

`func (o *PatchUserRequest) SetSchemas(v []string)`

SetSchemas sets Schemas field to given value.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


