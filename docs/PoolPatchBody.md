# PoolPatchBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Pool** | Pointer to **string** |  | [optional] 
**Slots** | Pointer to **int32** | Number of slots. Use -1 for unlimited. | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**IncludeDeferred** | Pointer to **bool** |  | [optional] 
**TeamName** | Pointer to **string** |  | [optional] 

## Methods

### NewPoolPatchBody

`func NewPoolPatchBody() *PoolPatchBody`

NewPoolPatchBody instantiates a new PoolPatchBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPoolPatchBodyWithDefaults

`func NewPoolPatchBodyWithDefaults() *PoolPatchBody`

NewPoolPatchBodyWithDefaults instantiates a new PoolPatchBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPool

`func (o *PoolPatchBody) GetPool() string`

GetPool returns the Pool field if non-nil, zero value otherwise.

### GetPoolOk

`func (o *PoolPatchBody) GetPoolOk() (*string, bool)`

GetPoolOk returns a tuple with the Pool field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPool

`func (o *PoolPatchBody) SetPool(v string)`

SetPool sets Pool field to given value.

### HasPool

`func (o *PoolPatchBody) HasPool() bool`

HasPool returns a boolean if a field has been set.

### GetSlots

`func (o *PoolPatchBody) GetSlots() int32`

GetSlots returns the Slots field if non-nil, zero value otherwise.

### GetSlotsOk

`func (o *PoolPatchBody) GetSlotsOk() (*int32, bool)`

GetSlotsOk returns a tuple with the Slots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlots

`func (o *PoolPatchBody) SetSlots(v int32)`

SetSlots sets Slots field to given value.

### HasSlots

`func (o *PoolPatchBody) HasSlots() bool`

HasSlots returns a boolean if a field has been set.

### GetDescription

`func (o *PoolPatchBody) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *PoolPatchBody) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *PoolPatchBody) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *PoolPatchBody) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetIncludeDeferred

`func (o *PoolPatchBody) GetIncludeDeferred() bool`

GetIncludeDeferred returns the IncludeDeferred field if non-nil, zero value otherwise.

### GetIncludeDeferredOk

`func (o *PoolPatchBody) GetIncludeDeferredOk() (*bool, bool)`

GetIncludeDeferredOk returns a tuple with the IncludeDeferred field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeDeferred

`func (o *PoolPatchBody) SetIncludeDeferred(v bool)`

SetIncludeDeferred sets IncludeDeferred field to given value.

### HasIncludeDeferred

`func (o *PoolPatchBody) HasIncludeDeferred() bool`

HasIncludeDeferred returns a boolean if a field has been set.

### GetTeamName

`func (o *PoolPatchBody) GetTeamName() string`

GetTeamName returns the TeamName field if non-nil, zero value otherwise.

### GetTeamNameOk

`func (o *PoolPatchBody) GetTeamNameOk() (*string, bool)`

GetTeamNameOk returns a tuple with the TeamName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamName

`func (o *PoolPatchBody) SetTeamName(v string)`

SetTeamName sets TeamName field to given value.

### HasTeamName

`func (o *PoolPatchBody) HasTeamName() bool`

HasTeamName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


