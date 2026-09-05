# DAGRunsBatchBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderBy** | Pointer to **NullableString** |  | [optional] 
**PageOffset** | Pointer to **int32** |  | [optional] [default to 0]
**PageLimit** | Pointer to **int32** |  | [optional] [default to 100]
**DagIds** | Pointer to **[]string** |  | [optional] 
**States** | Pointer to [**[]DagRunState**](DagRunState.md) |  | [optional] 
**RunAfterGte** | Pointer to **NullableTime** |  | [optional] 
**RunAfterGt** | Pointer to **NullableTime** |  | [optional] 
**RunAfterLte** | Pointer to **NullableTime** |  | [optional] 
**RunAfterLt** | Pointer to **NullableTime** |  | [optional] 
**LogicalDateGte** | Pointer to **NullableTime** |  | [optional] 
**LogicalDateGt** | Pointer to **NullableTime** |  | [optional] 
**LogicalDateLte** | Pointer to **NullableTime** |  | [optional] 
**LogicalDateLt** | Pointer to **NullableTime** |  | [optional] 
**StartDateGte** | Pointer to **NullableTime** |  | [optional] 
**StartDateGt** | Pointer to **NullableTime** |  | [optional] 
**StartDateLte** | Pointer to **NullableTime** |  | [optional] 
**StartDateLt** | Pointer to **NullableTime** |  | [optional] 
**EndDateGte** | Pointer to **NullableTime** |  | [optional] 
**EndDateGt** | Pointer to **NullableTime** |  | [optional] 
**EndDateLte** | Pointer to **NullableTime** |  | [optional] 
**EndDateLt** | Pointer to **NullableTime** |  | [optional] 
**DurationGte** | Pointer to **NullableFloat32** |  | [optional] 
**DurationGt** | Pointer to **NullableFloat32** |  | [optional] 
**DurationLte** | Pointer to **NullableFloat32** |  | [optional] 
**DurationLt** | Pointer to **NullableFloat32** |  | [optional] 
**ConfContains** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewDAGRunsBatchBody

`func NewDAGRunsBatchBody() *DAGRunsBatchBody`

NewDAGRunsBatchBody instantiates a new DAGRunsBatchBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDAGRunsBatchBodyWithDefaults

`func NewDAGRunsBatchBodyWithDefaults() *DAGRunsBatchBody`

NewDAGRunsBatchBodyWithDefaults instantiates a new DAGRunsBatchBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOrderBy

`func (o *DAGRunsBatchBody) GetOrderBy() string`

GetOrderBy returns the OrderBy field if non-nil, zero value otherwise.

### GetOrderByOk

`func (o *DAGRunsBatchBody) GetOrderByOk() (*string, bool)`

GetOrderByOk returns a tuple with the OrderBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrderBy

`func (o *DAGRunsBatchBody) SetOrderBy(v string)`

SetOrderBy sets OrderBy field to given value.

### HasOrderBy

`func (o *DAGRunsBatchBody) HasOrderBy() bool`

HasOrderBy returns a boolean if a field has been set.

### SetOrderByNil

`func (o *DAGRunsBatchBody) SetOrderByNil(b bool)`

 SetOrderByNil sets the value for OrderBy to be an explicit nil

### UnsetOrderBy
`func (o *DAGRunsBatchBody) UnsetOrderBy()`

UnsetOrderBy ensures that no value is present for OrderBy, not even an explicit nil
### GetPageOffset

`func (o *DAGRunsBatchBody) GetPageOffset() int32`

GetPageOffset returns the PageOffset field if non-nil, zero value otherwise.

### GetPageOffsetOk

`func (o *DAGRunsBatchBody) GetPageOffsetOk() (*int32, bool)`

GetPageOffsetOk returns a tuple with the PageOffset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageOffset

`func (o *DAGRunsBatchBody) SetPageOffset(v int32)`

SetPageOffset sets PageOffset field to given value.

### HasPageOffset

`func (o *DAGRunsBatchBody) HasPageOffset() bool`

HasPageOffset returns a boolean if a field has been set.

### GetPageLimit

`func (o *DAGRunsBatchBody) GetPageLimit() int32`

GetPageLimit returns the PageLimit field if non-nil, zero value otherwise.

### GetPageLimitOk

`func (o *DAGRunsBatchBody) GetPageLimitOk() (*int32, bool)`

GetPageLimitOk returns a tuple with the PageLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageLimit

`func (o *DAGRunsBatchBody) SetPageLimit(v int32)`

SetPageLimit sets PageLimit field to given value.

### HasPageLimit

`func (o *DAGRunsBatchBody) HasPageLimit() bool`

HasPageLimit returns a boolean if a field has been set.

### GetDagIds

`func (o *DAGRunsBatchBody) GetDagIds() []string`

GetDagIds returns the DagIds field if non-nil, zero value otherwise.

### GetDagIdsOk

`func (o *DAGRunsBatchBody) GetDagIdsOk() (*[]string, bool)`

GetDagIdsOk returns a tuple with the DagIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagIds

`func (o *DAGRunsBatchBody) SetDagIds(v []string)`

SetDagIds sets DagIds field to given value.

### HasDagIds

`func (o *DAGRunsBatchBody) HasDagIds() bool`

HasDagIds returns a boolean if a field has been set.

### SetDagIdsNil

`func (o *DAGRunsBatchBody) SetDagIdsNil(b bool)`

 SetDagIdsNil sets the value for DagIds to be an explicit nil

### UnsetDagIds
`func (o *DAGRunsBatchBody) UnsetDagIds()`

UnsetDagIds ensures that no value is present for DagIds, not even an explicit nil
### GetStates

`func (o *DAGRunsBatchBody) GetStates() []*DagRunState`

GetStates returns the States field if non-nil, zero value otherwise.

### GetStatesOk

`func (o *DAGRunsBatchBody) GetStatesOk() (*[]*DagRunState, bool)`

GetStatesOk returns a tuple with the States field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStates

`func (o *DAGRunsBatchBody) SetStates(v []*DagRunState)`

SetStates sets States field to given value.

### HasStates

`func (o *DAGRunsBatchBody) HasStates() bool`

HasStates returns a boolean if a field has been set.

### SetStatesNil

`func (o *DAGRunsBatchBody) SetStatesNil(b bool)`

 SetStatesNil sets the value for States to be an explicit nil

### UnsetStates
`func (o *DAGRunsBatchBody) UnsetStates()`

UnsetStates ensures that no value is present for States, not even an explicit nil
### GetRunAfterGte

`func (o *DAGRunsBatchBody) GetRunAfterGte() time.Time`

GetRunAfterGte returns the RunAfterGte field if non-nil, zero value otherwise.

### GetRunAfterGteOk

`func (o *DAGRunsBatchBody) GetRunAfterGteOk() (*time.Time, bool)`

GetRunAfterGteOk returns a tuple with the RunAfterGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfterGte

`func (o *DAGRunsBatchBody) SetRunAfterGte(v time.Time)`

SetRunAfterGte sets RunAfterGte field to given value.

### HasRunAfterGte

`func (o *DAGRunsBatchBody) HasRunAfterGte() bool`

HasRunAfterGte returns a boolean if a field has been set.

### SetRunAfterGteNil

`func (o *DAGRunsBatchBody) SetRunAfterGteNil(b bool)`

 SetRunAfterGteNil sets the value for RunAfterGte to be an explicit nil

### UnsetRunAfterGte
`func (o *DAGRunsBatchBody) UnsetRunAfterGte()`

UnsetRunAfterGte ensures that no value is present for RunAfterGte, not even an explicit nil
### GetRunAfterGt

`func (o *DAGRunsBatchBody) GetRunAfterGt() time.Time`

GetRunAfterGt returns the RunAfterGt field if non-nil, zero value otherwise.

### GetRunAfterGtOk

`func (o *DAGRunsBatchBody) GetRunAfterGtOk() (*time.Time, bool)`

GetRunAfterGtOk returns a tuple with the RunAfterGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfterGt

`func (o *DAGRunsBatchBody) SetRunAfterGt(v time.Time)`

SetRunAfterGt sets RunAfterGt field to given value.

### HasRunAfterGt

`func (o *DAGRunsBatchBody) HasRunAfterGt() bool`

HasRunAfterGt returns a boolean if a field has been set.

### SetRunAfterGtNil

`func (o *DAGRunsBatchBody) SetRunAfterGtNil(b bool)`

 SetRunAfterGtNil sets the value for RunAfterGt to be an explicit nil

### UnsetRunAfterGt
`func (o *DAGRunsBatchBody) UnsetRunAfterGt()`

UnsetRunAfterGt ensures that no value is present for RunAfterGt, not even an explicit nil
### GetRunAfterLte

`func (o *DAGRunsBatchBody) GetRunAfterLte() time.Time`

GetRunAfterLte returns the RunAfterLte field if non-nil, zero value otherwise.

### GetRunAfterLteOk

`func (o *DAGRunsBatchBody) GetRunAfterLteOk() (*time.Time, bool)`

GetRunAfterLteOk returns a tuple with the RunAfterLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfterLte

`func (o *DAGRunsBatchBody) SetRunAfterLte(v time.Time)`

SetRunAfterLte sets RunAfterLte field to given value.

### HasRunAfterLte

`func (o *DAGRunsBatchBody) HasRunAfterLte() bool`

HasRunAfterLte returns a boolean if a field has been set.

### SetRunAfterLteNil

`func (o *DAGRunsBatchBody) SetRunAfterLteNil(b bool)`

 SetRunAfterLteNil sets the value for RunAfterLte to be an explicit nil

### UnsetRunAfterLte
`func (o *DAGRunsBatchBody) UnsetRunAfterLte()`

UnsetRunAfterLte ensures that no value is present for RunAfterLte, not even an explicit nil
### GetRunAfterLt

`func (o *DAGRunsBatchBody) GetRunAfterLt() time.Time`

GetRunAfterLt returns the RunAfterLt field if non-nil, zero value otherwise.

### GetRunAfterLtOk

`func (o *DAGRunsBatchBody) GetRunAfterLtOk() (*time.Time, bool)`

GetRunAfterLtOk returns a tuple with the RunAfterLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfterLt

`func (o *DAGRunsBatchBody) SetRunAfterLt(v time.Time)`

SetRunAfterLt sets RunAfterLt field to given value.

### HasRunAfterLt

`func (o *DAGRunsBatchBody) HasRunAfterLt() bool`

HasRunAfterLt returns a boolean if a field has been set.

### SetRunAfterLtNil

`func (o *DAGRunsBatchBody) SetRunAfterLtNil(b bool)`

 SetRunAfterLtNil sets the value for RunAfterLt to be an explicit nil

### UnsetRunAfterLt
`func (o *DAGRunsBatchBody) UnsetRunAfterLt()`

UnsetRunAfterLt ensures that no value is present for RunAfterLt, not even an explicit nil
### GetLogicalDateGte

`func (o *DAGRunsBatchBody) GetLogicalDateGte() time.Time`

GetLogicalDateGte returns the LogicalDateGte field if non-nil, zero value otherwise.

### GetLogicalDateGteOk

`func (o *DAGRunsBatchBody) GetLogicalDateGteOk() (*time.Time, bool)`

GetLogicalDateGteOk returns a tuple with the LogicalDateGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDateGte

`func (o *DAGRunsBatchBody) SetLogicalDateGte(v time.Time)`

SetLogicalDateGte sets LogicalDateGte field to given value.

### HasLogicalDateGte

`func (o *DAGRunsBatchBody) HasLogicalDateGte() bool`

HasLogicalDateGte returns a boolean if a field has been set.

### SetLogicalDateGteNil

`func (o *DAGRunsBatchBody) SetLogicalDateGteNil(b bool)`

 SetLogicalDateGteNil sets the value for LogicalDateGte to be an explicit nil

### UnsetLogicalDateGte
`func (o *DAGRunsBatchBody) UnsetLogicalDateGte()`

UnsetLogicalDateGte ensures that no value is present for LogicalDateGte, not even an explicit nil
### GetLogicalDateGt

`func (o *DAGRunsBatchBody) GetLogicalDateGt() time.Time`

GetLogicalDateGt returns the LogicalDateGt field if non-nil, zero value otherwise.

### GetLogicalDateGtOk

`func (o *DAGRunsBatchBody) GetLogicalDateGtOk() (*time.Time, bool)`

GetLogicalDateGtOk returns a tuple with the LogicalDateGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDateGt

`func (o *DAGRunsBatchBody) SetLogicalDateGt(v time.Time)`

SetLogicalDateGt sets LogicalDateGt field to given value.

### HasLogicalDateGt

`func (o *DAGRunsBatchBody) HasLogicalDateGt() bool`

HasLogicalDateGt returns a boolean if a field has been set.

### SetLogicalDateGtNil

`func (o *DAGRunsBatchBody) SetLogicalDateGtNil(b bool)`

 SetLogicalDateGtNil sets the value for LogicalDateGt to be an explicit nil

### UnsetLogicalDateGt
`func (o *DAGRunsBatchBody) UnsetLogicalDateGt()`

UnsetLogicalDateGt ensures that no value is present for LogicalDateGt, not even an explicit nil
### GetLogicalDateLte

`func (o *DAGRunsBatchBody) GetLogicalDateLte() time.Time`

GetLogicalDateLte returns the LogicalDateLte field if non-nil, zero value otherwise.

### GetLogicalDateLteOk

`func (o *DAGRunsBatchBody) GetLogicalDateLteOk() (*time.Time, bool)`

GetLogicalDateLteOk returns a tuple with the LogicalDateLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDateLte

`func (o *DAGRunsBatchBody) SetLogicalDateLte(v time.Time)`

SetLogicalDateLte sets LogicalDateLte field to given value.

### HasLogicalDateLte

`func (o *DAGRunsBatchBody) HasLogicalDateLte() bool`

HasLogicalDateLte returns a boolean if a field has been set.

### SetLogicalDateLteNil

`func (o *DAGRunsBatchBody) SetLogicalDateLteNil(b bool)`

 SetLogicalDateLteNil sets the value for LogicalDateLte to be an explicit nil

### UnsetLogicalDateLte
`func (o *DAGRunsBatchBody) UnsetLogicalDateLte()`

UnsetLogicalDateLte ensures that no value is present for LogicalDateLte, not even an explicit nil
### GetLogicalDateLt

`func (o *DAGRunsBatchBody) GetLogicalDateLt() time.Time`

GetLogicalDateLt returns the LogicalDateLt field if non-nil, zero value otherwise.

### GetLogicalDateLtOk

`func (o *DAGRunsBatchBody) GetLogicalDateLtOk() (*time.Time, bool)`

GetLogicalDateLtOk returns a tuple with the LogicalDateLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDateLt

`func (o *DAGRunsBatchBody) SetLogicalDateLt(v time.Time)`

SetLogicalDateLt sets LogicalDateLt field to given value.

### HasLogicalDateLt

`func (o *DAGRunsBatchBody) HasLogicalDateLt() bool`

HasLogicalDateLt returns a boolean if a field has been set.

### SetLogicalDateLtNil

`func (o *DAGRunsBatchBody) SetLogicalDateLtNil(b bool)`

 SetLogicalDateLtNil sets the value for LogicalDateLt to be an explicit nil

### UnsetLogicalDateLt
`func (o *DAGRunsBatchBody) UnsetLogicalDateLt()`

UnsetLogicalDateLt ensures that no value is present for LogicalDateLt, not even an explicit nil
### GetStartDateGte

`func (o *DAGRunsBatchBody) GetStartDateGte() time.Time`

GetStartDateGte returns the StartDateGte field if non-nil, zero value otherwise.

### GetStartDateGteOk

`func (o *DAGRunsBatchBody) GetStartDateGteOk() (*time.Time, bool)`

GetStartDateGteOk returns a tuple with the StartDateGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDateGte

`func (o *DAGRunsBatchBody) SetStartDateGte(v time.Time)`

SetStartDateGte sets StartDateGte field to given value.

### HasStartDateGte

`func (o *DAGRunsBatchBody) HasStartDateGte() bool`

HasStartDateGte returns a boolean if a field has been set.

### SetStartDateGteNil

`func (o *DAGRunsBatchBody) SetStartDateGteNil(b bool)`

 SetStartDateGteNil sets the value for StartDateGte to be an explicit nil

### UnsetStartDateGte
`func (o *DAGRunsBatchBody) UnsetStartDateGte()`

UnsetStartDateGte ensures that no value is present for StartDateGte, not even an explicit nil
### GetStartDateGt

`func (o *DAGRunsBatchBody) GetStartDateGt() time.Time`

GetStartDateGt returns the StartDateGt field if non-nil, zero value otherwise.

### GetStartDateGtOk

`func (o *DAGRunsBatchBody) GetStartDateGtOk() (*time.Time, bool)`

GetStartDateGtOk returns a tuple with the StartDateGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDateGt

`func (o *DAGRunsBatchBody) SetStartDateGt(v time.Time)`

SetStartDateGt sets StartDateGt field to given value.

### HasStartDateGt

`func (o *DAGRunsBatchBody) HasStartDateGt() bool`

HasStartDateGt returns a boolean if a field has been set.

### SetStartDateGtNil

`func (o *DAGRunsBatchBody) SetStartDateGtNil(b bool)`

 SetStartDateGtNil sets the value for StartDateGt to be an explicit nil

### UnsetStartDateGt
`func (o *DAGRunsBatchBody) UnsetStartDateGt()`

UnsetStartDateGt ensures that no value is present for StartDateGt, not even an explicit nil
### GetStartDateLte

`func (o *DAGRunsBatchBody) GetStartDateLte() time.Time`

GetStartDateLte returns the StartDateLte field if non-nil, zero value otherwise.

### GetStartDateLteOk

`func (o *DAGRunsBatchBody) GetStartDateLteOk() (*time.Time, bool)`

GetStartDateLteOk returns a tuple with the StartDateLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDateLte

`func (o *DAGRunsBatchBody) SetStartDateLte(v time.Time)`

SetStartDateLte sets StartDateLte field to given value.

### HasStartDateLte

`func (o *DAGRunsBatchBody) HasStartDateLte() bool`

HasStartDateLte returns a boolean if a field has been set.

### SetStartDateLteNil

`func (o *DAGRunsBatchBody) SetStartDateLteNil(b bool)`

 SetStartDateLteNil sets the value for StartDateLte to be an explicit nil

### UnsetStartDateLte
`func (o *DAGRunsBatchBody) UnsetStartDateLte()`

UnsetStartDateLte ensures that no value is present for StartDateLte, not even an explicit nil
### GetStartDateLt

`func (o *DAGRunsBatchBody) GetStartDateLt() time.Time`

GetStartDateLt returns the StartDateLt field if non-nil, zero value otherwise.

### GetStartDateLtOk

`func (o *DAGRunsBatchBody) GetStartDateLtOk() (*time.Time, bool)`

GetStartDateLtOk returns a tuple with the StartDateLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDateLt

`func (o *DAGRunsBatchBody) SetStartDateLt(v time.Time)`

SetStartDateLt sets StartDateLt field to given value.

### HasStartDateLt

`func (o *DAGRunsBatchBody) HasStartDateLt() bool`

HasStartDateLt returns a boolean if a field has been set.

### SetStartDateLtNil

`func (o *DAGRunsBatchBody) SetStartDateLtNil(b bool)`

 SetStartDateLtNil sets the value for StartDateLt to be an explicit nil

### UnsetStartDateLt
`func (o *DAGRunsBatchBody) UnsetStartDateLt()`

UnsetStartDateLt ensures that no value is present for StartDateLt, not even an explicit nil
### GetEndDateGte

`func (o *DAGRunsBatchBody) GetEndDateGte() time.Time`

GetEndDateGte returns the EndDateGte field if non-nil, zero value otherwise.

### GetEndDateGteOk

`func (o *DAGRunsBatchBody) GetEndDateGteOk() (*time.Time, bool)`

GetEndDateGteOk returns a tuple with the EndDateGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDateGte

`func (o *DAGRunsBatchBody) SetEndDateGte(v time.Time)`

SetEndDateGte sets EndDateGte field to given value.

### HasEndDateGte

`func (o *DAGRunsBatchBody) HasEndDateGte() bool`

HasEndDateGte returns a boolean if a field has been set.

### SetEndDateGteNil

`func (o *DAGRunsBatchBody) SetEndDateGteNil(b bool)`

 SetEndDateGteNil sets the value for EndDateGte to be an explicit nil

### UnsetEndDateGte
`func (o *DAGRunsBatchBody) UnsetEndDateGte()`

UnsetEndDateGte ensures that no value is present for EndDateGte, not even an explicit nil
### GetEndDateGt

`func (o *DAGRunsBatchBody) GetEndDateGt() time.Time`

GetEndDateGt returns the EndDateGt field if non-nil, zero value otherwise.

### GetEndDateGtOk

`func (o *DAGRunsBatchBody) GetEndDateGtOk() (*time.Time, bool)`

GetEndDateGtOk returns a tuple with the EndDateGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDateGt

`func (o *DAGRunsBatchBody) SetEndDateGt(v time.Time)`

SetEndDateGt sets EndDateGt field to given value.

### HasEndDateGt

`func (o *DAGRunsBatchBody) HasEndDateGt() bool`

HasEndDateGt returns a boolean if a field has been set.

### SetEndDateGtNil

`func (o *DAGRunsBatchBody) SetEndDateGtNil(b bool)`

 SetEndDateGtNil sets the value for EndDateGt to be an explicit nil

### UnsetEndDateGt
`func (o *DAGRunsBatchBody) UnsetEndDateGt()`

UnsetEndDateGt ensures that no value is present for EndDateGt, not even an explicit nil
### GetEndDateLte

`func (o *DAGRunsBatchBody) GetEndDateLte() time.Time`

GetEndDateLte returns the EndDateLte field if non-nil, zero value otherwise.

### GetEndDateLteOk

`func (o *DAGRunsBatchBody) GetEndDateLteOk() (*time.Time, bool)`

GetEndDateLteOk returns a tuple with the EndDateLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDateLte

`func (o *DAGRunsBatchBody) SetEndDateLte(v time.Time)`

SetEndDateLte sets EndDateLte field to given value.

### HasEndDateLte

`func (o *DAGRunsBatchBody) HasEndDateLte() bool`

HasEndDateLte returns a boolean if a field has been set.

### SetEndDateLteNil

`func (o *DAGRunsBatchBody) SetEndDateLteNil(b bool)`

 SetEndDateLteNil sets the value for EndDateLte to be an explicit nil

### UnsetEndDateLte
`func (o *DAGRunsBatchBody) UnsetEndDateLte()`

UnsetEndDateLte ensures that no value is present for EndDateLte, not even an explicit nil
### GetEndDateLt

`func (o *DAGRunsBatchBody) GetEndDateLt() time.Time`

GetEndDateLt returns the EndDateLt field if non-nil, zero value otherwise.

### GetEndDateLtOk

`func (o *DAGRunsBatchBody) GetEndDateLtOk() (*time.Time, bool)`

GetEndDateLtOk returns a tuple with the EndDateLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDateLt

`func (o *DAGRunsBatchBody) SetEndDateLt(v time.Time)`

SetEndDateLt sets EndDateLt field to given value.

### HasEndDateLt

`func (o *DAGRunsBatchBody) HasEndDateLt() bool`

HasEndDateLt returns a boolean if a field has been set.

### SetEndDateLtNil

`func (o *DAGRunsBatchBody) SetEndDateLtNil(b bool)`

 SetEndDateLtNil sets the value for EndDateLt to be an explicit nil

### UnsetEndDateLt
`func (o *DAGRunsBatchBody) UnsetEndDateLt()`

UnsetEndDateLt ensures that no value is present for EndDateLt, not even an explicit nil
### GetDurationGte

`func (o *DAGRunsBatchBody) GetDurationGte() float32`

GetDurationGte returns the DurationGte field if non-nil, zero value otherwise.

### GetDurationGteOk

`func (o *DAGRunsBatchBody) GetDurationGteOk() (*float32, bool)`

GetDurationGteOk returns a tuple with the DurationGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationGte

`func (o *DAGRunsBatchBody) SetDurationGte(v float32)`

SetDurationGte sets DurationGte field to given value.

### HasDurationGte

`func (o *DAGRunsBatchBody) HasDurationGte() bool`

HasDurationGte returns a boolean if a field has been set.

### SetDurationGteNil

`func (o *DAGRunsBatchBody) SetDurationGteNil(b bool)`

 SetDurationGteNil sets the value for DurationGte to be an explicit nil

### UnsetDurationGte
`func (o *DAGRunsBatchBody) UnsetDurationGte()`

UnsetDurationGte ensures that no value is present for DurationGte, not even an explicit nil
### GetDurationGt

`func (o *DAGRunsBatchBody) GetDurationGt() float32`

GetDurationGt returns the DurationGt field if non-nil, zero value otherwise.

### GetDurationGtOk

`func (o *DAGRunsBatchBody) GetDurationGtOk() (*float32, bool)`

GetDurationGtOk returns a tuple with the DurationGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationGt

`func (o *DAGRunsBatchBody) SetDurationGt(v float32)`

SetDurationGt sets DurationGt field to given value.

### HasDurationGt

`func (o *DAGRunsBatchBody) HasDurationGt() bool`

HasDurationGt returns a boolean if a field has been set.

### SetDurationGtNil

`func (o *DAGRunsBatchBody) SetDurationGtNil(b bool)`

 SetDurationGtNil sets the value for DurationGt to be an explicit nil

### UnsetDurationGt
`func (o *DAGRunsBatchBody) UnsetDurationGt()`

UnsetDurationGt ensures that no value is present for DurationGt, not even an explicit nil
### GetDurationLte

`func (o *DAGRunsBatchBody) GetDurationLte() float32`

GetDurationLte returns the DurationLte field if non-nil, zero value otherwise.

### GetDurationLteOk

`func (o *DAGRunsBatchBody) GetDurationLteOk() (*float32, bool)`

GetDurationLteOk returns a tuple with the DurationLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationLte

`func (o *DAGRunsBatchBody) SetDurationLte(v float32)`

SetDurationLte sets DurationLte field to given value.

### HasDurationLte

`func (o *DAGRunsBatchBody) HasDurationLte() bool`

HasDurationLte returns a boolean if a field has been set.

### SetDurationLteNil

`func (o *DAGRunsBatchBody) SetDurationLteNil(b bool)`

 SetDurationLteNil sets the value for DurationLte to be an explicit nil

### UnsetDurationLte
`func (o *DAGRunsBatchBody) UnsetDurationLte()`

UnsetDurationLte ensures that no value is present for DurationLte, not even an explicit nil
### GetDurationLt

`func (o *DAGRunsBatchBody) GetDurationLt() float32`

GetDurationLt returns the DurationLt field if non-nil, zero value otherwise.

### GetDurationLtOk

`func (o *DAGRunsBatchBody) GetDurationLtOk() (*float32, bool)`

GetDurationLtOk returns a tuple with the DurationLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationLt

`func (o *DAGRunsBatchBody) SetDurationLt(v float32)`

SetDurationLt sets DurationLt field to given value.

### HasDurationLt

`func (o *DAGRunsBatchBody) HasDurationLt() bool`

HasDurationLt returns a boolean if a field has been set.

### SetDurationLtNil

`func (o *DAGRunsBatchBody) SetDurationLtNil(b bool)`

 SetDurationLtNil sets the value for DurationLt to be an explicit nil

### UnsetDurationLt
`func (o *DAGRunsBatchBody) UnsetDurationLt()`

UnsetDurationLt ensures that no value is present for DurationLt, not even an explicit nil
### GetConfContains

`func (o *DAGRunsBatchBody) GetConfContains() string`

GetConfContains returns the ConfContains field if non-nil, zero value otherwise.

### GetConfContainsOk

`func (o *DAGRunsBatchBody) GetConfContainsOk() (*string, bool)`

GetConfContainsOk returns a tuple with the ConfContains field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfContains

`func (o *DAGRunsBatchBody) SetConfContains(v string)`

SetConfContains sets ConfContains field to given value.

### HasConfContains

`func (o *DAGRunsBatchBody) HasConfContains() bool`

HasConfContains returns a boolean if a field has been set.

### SetConfContainsNil

`func (o *DAGRunsBatchBody) SetConfContainsNil(b bool)`

 SetConfContainsNil sets the value for ConfContains to be an explicit nil

### UnsetConfContains
`func (o *DAGRunsBatchBody) UnsetConfContains()`

UnsetConfContains ensures that no value is present for ConfContains, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


