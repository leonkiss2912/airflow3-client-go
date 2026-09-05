# DAGRunsBatchBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**OrderBy** | Pointer to **string** |  | [optional] 
**PageOffset** | Pointer to **int32** |  | [optional] [default to 0]
**PageLimit** | Pointer to **int32** |  | [optional] [default to 100]
**DagIds** | Pointer to **[]string** |  | [optional] 
**States** | Pointer to [**[]DagRunState**](DagRunState.md) |  | [optional] 
**RunAfterGte** | Pointer to **time.Time** |  | [optional] 
**RunAfterGt** | Pointer to **time.Time** |  | [optional] 
**RunAfterLte** | Pointer to **time.Time** |  | [optional] 
**RunAfterLt** | Pointer to **time.Time** |  | [optional] 
**LogicalDateGte** | Pointer to **time.Time** |  | [optional] 
**LogicalDateGt** | Pointer to **time.Time** |  | [optional] 
**LogicalDateLte** | Pointer to **time.Time** |  | [optional] 
**LogicalDateLt** | Pointer to **time.Time** |  | [optional] 
**StartDateGte** | Pointer to **time.Time** |  | [optional] 
**StartDateGt** | Pointer to **time.Time** |  | [optional] 
**StartDateLte** | Pointer to **time.Time** |  | [optional] 
**StartDateLt** | Pointer to **time.Time** |  | [optional] 
**EndDateGte** | Pointer to **time.Time** |  | [optional] 
**EndDateGt** | Pointer to **time.Time** |  | [optional] 
**EndDateLte** | Pointer to **time.Time** |  | [optional] 
**EndDateLt** | Pointer to **time.Time** |  | [optional] 
**DurationGte** | Pointer to **float32** |  | [optional] 
**DurationGt** | Pointer to **float32** |  | [optional] 
**DurationLte** | Pointer to **float32** |  | [optional] 
**DurationLt** | Pointer to **float32** |  | [optional] 
**ConfContains** | Pointer to **string** |  | [optional] 

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

### GetStates

`func (o *DAGRunsBatchBody) GetStates() []DagRunState`

GetStates returns the States field if non-nil, zero value otherwise.

### GetStatesOk

`func (o *DAGRunsBatchBody) GetStatesOk() (*[]DagRunState, bool)`

GetStatesOk returns a tuple with the States field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStates

`func (o *DAGRunsBatchBody) SetStates(v []DagRunState)`

SetStates sets States field to given value.

### HasStates

`func (o *DAGRunsBatchBody) HasStates() bool`

HasStates returns a boolean if a field has been set.

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


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


