# ActionsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Action** | **string** | The action to be performed on the entities. | 
**Entities** | [**[]EntitiesInner**](EntitiesInner.md) | A list of entity id/key or entity objects to be deleted. | 
**ActionOnExistence** | Pointer to [**BulkActionOnExistence**](BulkActionOnExistence.md) |  | [optional] [default to FAIL]
**UpdateMask** | Pointer to **[]string** | A list of field names to update for each entity.Only these fields will be applied from the request body to the database model.Any extra fields provided will be ignored. | [optional] 
**ActionOnNonExistence** | Pointer to [**BulkActionNotOnExistence**](BulkActionNotOnExistence.md) |  | [optional] [default to FAIL]

## Methods

### NewActionsInner

`func NewActionsInner(action string, entities []EntitiesInner, ) *ActionsInner`

NewActionsInner instantiates a new ActionsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewActionsInnerWithDefaults

`func NewActionsInnerWithDefaults() *ActionsInner`

NewActionsInnerWithDefaults instantiates a new ActionsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAction

`func (o *ActionsInner) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *ActionsInner) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *ActionsInner) SetAction(v string)`

SetAction sets Action field to given value.


### GetEntities

`func (o *ActionsInner) GetEntities() []EntitiesInner`

GetEntities returns the Entities field if non-nil, zero value otherwise.

### GetEntitiesOk

`func (o *ActionsInner) GetEntitiesOk() (*[]EntitiesInner, bool)`

GetEntitiesOk returns a tuple with the Entities field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntities

`func (o *ActionsInner) SetEntities(v []EntitiesInner)`

SetEntities sets Entities field to given value.


### GetActionOnExistence

`func (o *ActionsInner) GetActionOnExistence() BulkActionOnExistence`

GetActionOnExistence returns the ActionOnExistence field if non-nil, zero value otherwise.

### GetActionOnExistenceOk

`func (o *ActionsInner) GetActionOnExistenceOk() (*BulkActionOnExistence, bool)`

GetActionOnExistenceOk returns a tuple with the ActionOnExistence field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionOnExistence

`func (o *ActionsInner) SetActionOnExistence(v BulkActionOnExistence)`

SetActionOnExistence sets ActionOnExistence field to given value.

### HasActionOnExistence

`func (o *ActionsInner) HasActionOnExistence() bool`

HasActionOnExistence returns a boolean if a field has been set.

### GetUpdateMask

`func (o *ActionsInner) GetUpdateMask() []string`

GetUpdateMask returns the UpdateMask field if non-nil, zero value otherwise.

### GetUpdateMaskOk

`func (o *ActionsInner) GetUpdateMaskOk() (*[]string, bool)`

GetUpdateMaskOk returns a tuple with the UpdateMask field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdateMask

`func (o *ActionsInner) SetUpdateMask(v []string)`

SetUpdateMask sets UpdateMask field to given value.

### HasUpdateMask

`func (o *ActionsInner) HasUpdateMask() bool`

HasUpdateMask returns a boolean if a field has been set.

### GetActionOnNonExistence

`func (o *ActionsInner) GetActionOnNonExistence() BulkActionNotOnExistence`

GetActionOnNonExistence returns the ActionOnNonExistence field if non-nil, zero value otherwise.

### GetActionOnNonExistenceOk

`func (o *ActionsInner) GetActionOnNonExistenceOk() (*BulkActionNotOnExistence, bool)`

GetActionOnNonExistenceOk returns a tuple with the ActionOnNonExistence field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionOnNonExistence

`func (o *ActionsInner) SetActionOnNonExistence(v BulkActionNotOnExistence)`

SetActionOnNonExistence sets ActionOnNonExistence field to given value.

### HasActionOnNonExistence

`func (o *ActionsInner) HasActionOnNonExistence() bool`

HasActionOnNonExistence returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


