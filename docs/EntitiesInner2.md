# EntitiesInner2

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Slots** | **int32** | Number of slots. Use -1 for unlimited. | 
**Description** | Pointer to **string** |  | [optional] 
**IncludeDeferred** | Pointer to **bool** |  | [optional] [default to false]
**TeamName** | Pointer to **string** |  | [optional] 

## Methods

### NewEntitiesInner2

`func NewEntitiesInner2(name string, slots int32, ) *EntitiesInner2`

NewEntitiesInner2 instantiates a new EntitiesInner2 object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntitiesInner2WithDefaults

`func NewEntitiesInner2WithDefaults() *EntitiesInner2`

NewEntitiesInner2WithDefaults instantiates a new EntitiesInner2 object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *EntitiesInner2) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EntitiesInner2) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EntitiesInner2) SetName(v string)`

SetName sets Name field to given value.


### GetSlots

`func (o *EntitiesInner2) GetSlots() int32`

GetSlots returns the Slots field if non-nil, zero value otherwise.

### GetSlotsOk

`func (o *EntitiesInner2) GetSlotsOk() (*int32, bool)`

GetSlotsOk returns a tuple with the Slots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlots

`func (o *EntitiesInner2) SetSlots(v int32)`

SetSlots sets Slots field to given value.


### GetDescription

`func (o *EntitiesInner2) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *EntitiesInner2) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *EntitiesInner2) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *EntitiesInner2) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetIncludeDeferred

`func (o *EntitiesInner2) GetIncludeDeferred() bool`

GetIncludeDeferred returns the IncludeDeferred field if non-nil, zero value otherwise.

### GetIncludeDeferredOk

`func (o *EntitiesInner2) GetIncludeDeferredOk() (*bool, bool)`

GetIncludeDeferredOk returns a tuple with the IncludeDeferred field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeDeferred

`func (o *EntitiesInner2) SetIncludeDeferred(v bool)`

SetIncludeDeferred sets IncludeDeferred field to given value.

### HasIncludeDeferred

`func (o *EntitiesInner2) HasIncludeDeferred() bool`

HasIncludeDeferred returns a boolean if a field has been set.

### GetTeamName

`func (o *EntitiesInner2) GetTeamName() string`

GetTeamName returns the TeamName field if non-nil, zero value otherwise.

### GetTeamNameOk

`func (o *EntitiesInner2) GetTeamNameOk() (*string, bool)`

GetTeamNameOk returns a tuple with the TeamName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamName

`func (o *EntitiesInner2) SetTeamName(v string)`

SetTeamName sets TeamName field to given value.

### HasTeamName

`func (o *EntitiesInner2) HasTeamName() bool`

HasTeamName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


