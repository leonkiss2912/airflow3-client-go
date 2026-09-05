# HITLDetailHistory

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Options** | **[]string** |  | 
**Subject** | **string** |  | 
**Body** | Pointer to **NullableString** |  | [optional] 
**Defaults** | Pointer to **[]string** |  | [optional] 
**Multiple** | Pointer to **bool** |  | [optional] [default to false]
**Params** | Pointer to **map[string]interface{}** |  | [optional] 
**AssignedUsers** | Pointer to [**[]HITLUser**](HITLUser.md) |  | [optional] 
**CreatedAt** | **time.Time** |  | 
**RespondedByUser** | Pointer to [**NullableHITLUser**](HITLUser.md) |  | [optional] 
**RespondedAt** | Pointer to **NullableTime** |  | [optional] 
**ChosenOptions** | Pointer to **[]string** |  | [optional] 
**ParamsInput** | Pointer to **map[string]interface{}** |  | [optional] 
**ResponseReceived** | Pointer to **bool** |  | [optional] [default to false]
**TaskInstance** | [**TaskInstanceHistoryResponse**](TaskInstanceHistoryResponse.md) |  | 

## Methods

### NewHITLDetailHistory

`func NewHITLDetailHistory(options []string, subject string, createdAt time.Time, taskInstance TaskInstanceHistoryResponse, ) *HITLDetailHistory`

NewHITLDetailHistory instantiates a new HITLDetailHistory object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHITLDetailHistoryWithDefaults

`func NewHITLDetailHistoryWithDefaults() *HITLDetailHistory`

NewHITLDetailHistoryWithDefaults instantiates a new HITLDetailHistory object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOptions

`func (o *HITLDetailHistory) GetOptions() []string`

GetOptions returns the Options field if non-nil, zero value otherwise.

### GetOptionsOk

`func (o *HITLDetailHistory) GetOptionsOk() (*[]string, bool)`

GetOptionsOk returns a tuple with the Options field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptions

`func (o *HITLDetailHistory) SetOptions(v []string)`

SetOptions sets Options field to given value.


### GetSubject

`func (o *HITLDetailHistory) GetSubject() string`

GetSubject returns the Subject field if non-nil, zero value otherwise.

### GetSubjectOk

`func (o *HITLDetailHistory) GetSubjectOk() (*string, bool)`

GetSubjectOk returns a tuple with the Subject field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubject

`func (o *HITLDetailHistory) SetSubject(v string)`

SetSubject sets Subject field to given value.


### GetBody

`func (o *HITLDetailHistory) GetBody() string`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *HITLDetailHistory) GetBodyOk() (*string, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *HITLDetailHistory) SetBody(v string)`

SetBody sets Body field to given value.

### HasBody

`func (o *HITLDetailHistory) HasBody() bool`

HasBody returns a boolean if a field has been set.

### SetBodyNil

`func (o *HITLDetailHistory) SetBodyNil(b bool)`

 SetBodyNil sets the value for Body to be an explicit nil

### UnsetBody
`func (o *HITLDetailHistory) UnsetBody()`

UnsetBody ensures that no value is present for Body, not even an explicit nil
### GetDefaults

`func (o *HITLDetailHistory) GetDefaults() []string`

GetDefaults returns the Defaults field if non-nil, zero value otherwise.

### GetDefaultsOk

`func (o *HITLDetailHistory) GetDefaultsOk() (*[]string, bool)`

GetDefaultsOk returns a tuple with the Defaults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaults

`func (o *HITLDetailHistory) SetDefaults(v []string)`

SetDefaults sets Defaults field to given value.

### HasDefaults

`func (o *HITLDetailHistory) HasDefaults() bool`

HasDefaults returns a boolean if a field has been set.

### SetDefaultsNil

`func (o *HITLDetailHistory) SetDefaultsNil(b bool)`

 SetDefaultsNil sets the value for Defaults to be an explicit nil

### UnsetDefaults
`func (o *HITLDetailHistory) UnsetDefaults()`

UnsetDefaults ensures that no value is present for Defaults, not even an explicit nil
### GetMultiple

`func (o *HITLDetailHistory) GetMultiple() bool`

GetMultiple returns the Multiple field if non-nil, zero value otherwise.

### GetMultipleOk

`func (o *HITLDetailHistory) GetMultipleOk() (*bool, bool)`

GetMultipleOk returns a tuple with the Multiple field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMultiple

`func (o *HITLDetailHistory) SetMultiple(v bool)`

SetMultiple sets Multiple field to given value.

### HasMultiple

`func (o *HITLDetailHistory) HasMultiple() bool`

HasMultiple returns a boolean if a field has been set.

### GetParams

`func (o *HITLDetailHistory) GetParams() map[string]interface{}`

GetParams returns the Params field if non-nil, zero value otherwise.

### GetParamsOk

`func (o *HITLDetailHistory) GetParamsOk() (*map[string]interface{}, bool)`

GetParamsOk returns a tuple with the Params field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParams

`func (o *HITLDetailHistory) SetParams(v map[string]interface{})`

SetParams sets Params field to given value.

### HasParams

`func (o *HITLDetailHistory) HasParams() bool`

HasParams returns a boolean if a field has been set.

### GetAssignedUsers

`func (o *HITLDetailHistory) GetAssignedUsers() []HITLUser`

GetAssignedUsers returns the AssignedUsers field if non-nil, zero value otherwise.

### GetAssignedUsersOk

`func (o *HITLDetailHistory) GetAssignedUsersOk() (*[]HITLUser, bool)`

GetAssignedUsersOk returns a tuple with the AssignedUsers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssignedUsers

`func (o *HITLDetailHistory) SetAssignedUsers(v []HITLUser)`

SetAssignedUsers sets AssignedUsers field to given value.

### HasAssignedUsers

`func (o *HITLDetailHistory) HasAssignedUsers() bool`

HasAssignedUsers returns a boolean if a field has been set.

### GetCreatedAt

`func (o *HITLDetailHistory) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *HITLDetailHistory) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *HITLDetailHistory) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetRespondedByUser

`func (o *HITLDetailHistory) GetRespondedByUser() HITLUser`

GetRespondedByUser returns the RespondedByUser field if non-nil, zero value otherwise.

### GetRespondedByUserOk

`func (o *HITLDetailHistory) GetRespondedByUserOk() (*HITLUser, bool)`

GetRespondedByUserOk returns a tuple with the RespondedByUser field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRespondedByUser

`func (o *HITLDetailHistory) SetRespondedByUser(v HITLUser)`

SetRespondedByUser sets RespondedByUser field to given value.

### HasRespondedByUser

`func (o *HITLDetailHistory) HasRespondedByUser() bool`

HasRespondedByUser returns a boolean if a field has been set.

### SetRespondedByUserNil

`func (o *HITLDetailHistory) SetRespondedByUserNil(b bool)`

 SetRespondedByUserNil sets the value for RespondedByUser to be an explicit nil

### UnsetRespondedByUser
`func (o *HITLDetailHistory) UnsetRespondedByUser()`

UnsetRespondedByUser ensures that no value is present for RespondedByUser, not even an explicit nil
### GetRespondedAt

`func (o *HITLDetailHistory) GetRespondedAt() time.Time`

GetRespondedAt returns the RespondedAt field if non-nil, zero value otherwise.

### GetRespondedAtOk

`func (o *HITLDetailHistory) GetRespondedAtOk() (*time.Time, bool)`

GetRespondedAtOk returns a tuple with the RespondedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRespondedAt

`func (o *HITLDetailHistory) SetRespondedAt(v time.Time)`

SetRespondedAt sets RespondedAt field to given value.

### HasRespondedAt

`func (o *HITLDetailHistory) HasRespondedAt() bool`

HasRespondedAt returns a boolean if a field has been set.

### SetRespondedAtNil

`func (o *HITLDetailHistory) SetRespondedAtNil(b bool)`

 SetRespondedAtNil sets the value for RespondedAt to be an explicit nil

### UnsetRespondedAt
`func (o *HITLDetailHistory) UnsetRespondedAt()`

UnsetRespondedAt ensures that no value is present for RespondedAt, not even an explicit nil
### GetChosenOptions

`func (o *HITLDetailHistory) GetChosenOptions() []string`

GetChosenOptions returns the ChosenOptions field if non-nil, zero value otherwise.

### GetChosenOptionsOk

`func (o *HITLDetailHistory) GetChosenOptionsOk() (*[]string, bool)`

GetChosenOptionsOk returns a tuple with the ChosenOptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChosenOptions

`func (o *HITLDetailHistory) SetChosenOptions(v []string)`

SetChosenOptions sets ChosenOptions field to given value.

### HasChosenOptions

`func (o *HITLDetailHistory) HasChosenOptions() bool`

HasChosenOptions returns a boolean if a field has been set.

### SetChosenOptionsNil

`func (o *HITLDetailHistory) SetChosenOptionsNil(b bool)`

 SetChosenOptionsNil sets the value for ChosenOptions to be an explicit nil

### UnsetChosenOptions
`func (o *HITLDetailHistory) UnsetChosenOptions()`

UnsetChosenOptions ensures that no value is present for ChosenOptions, not even an explicit nil
### GetParamsInput

`func (o *HITLDetailHistory) GetParamsInput() map[string]interface{}`

GetParamsInput returns the ParamsInput field if non-nil, zero value otherwise.

### GetParamsInputOk

`func (o *HITLDetailHistory) GetParamsInputOk() (*map[string]interface{}, bool)`

GetParamsInputOk returns a tuple with the ParamsInput field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParamsInput

`func (o *HITLDetailHistory) SetParamsInput(v map[string]interface{})`

SetParamsInput sets ParamsInput field to given value.

### HasParamsInput

`func (o *HITLDetailHistory) HasParamsInput() bool`

HasParamsInput returns a boolean if a field has been set.

### GetResponseReceived

`func (o *HITLDetailHistory) GetResponseReceived() bool`

GetResponseReceived returns the ResponseReceived field if non-nil, zero value otherwise.

### GetResponseReceivedOk

`func (o *HITLDetailHistory) GetResponseReceivedOk() (*bool, bool)`

GetResponseReceivedOk returns a tuple with the ResponseReceived field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseReceived

`func (o *HITLDetailHistory) SetResponseReceived(v bool)`

SetResponseReceived sets ResponseReceived field to given value.

### HasResponseReceived

`func (o *HITLDetailHistory) HasResponseReceived() bool`

HasResponseReceived returns a boolean if a field has been set.

### GetTaskInstance

`func (o *HITLDetailHistory) GetTaskInstance() TaskInstanceHistoryResponse`

GetTaskInstance returns the TaskInstance field if non-nil, zero value otherwise.

### GetTaskInstanceOk

`func (o *HITLDetailHistory) GetTaskInstanceOk() (*TaskInstanceHistoryResponse, bool)`

GetTaskInstanceOk returns a tuple with the TaskInstance field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskInstance

`func (o *HITLDetailHistory) SetTaskInstance(v TaskInstanceHistoryResponse)`

SetTaskInstance sets TaskInstance field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


