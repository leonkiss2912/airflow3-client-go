# TaskInstancesBatchBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DagIds** | Pointer to **[]string** |  | [optional] 
**DagRunIds** | Pointer to **[]string** |  | [optional] 
**TaskIds** | Pointer to **[]string** |  | [optional] 
**State** | Pointer to [**[]TaskInstanceState**](TaskInstanceState.md) |  | [optional] 
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
**Pool** | Pointer to **[]string** |  | [optional] 
**Queue** | Pointer to **[]string** |  | [optional] 
**Executor** | Pointer to **[]string** |  | [optional] 
**PageOffset** | Pointer to **int32** |  | [optional] [default to 0]
**PageLimit** | Pointer to **int32** |  | [optional] [default to 100]
**OrderBy** | Pointer to **string** |  | [optional] 

## Methods

### NewTaskInstancesBatchBody

`func NewTaskInstancesBatchBody() *TaskInstancesBatchBody`

NewTaskInstancesBatchBody instantiates a new TaskInstancesBatchBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaskInstancesBatchBodyWithDefaults

`func NewTaskInstancesBatchBodyWithDefaults() *TaskInstancesBatchBody`

NewTaskInstancesBatchBodyWithDefaults instantiates a new TaskInstancesBatchBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDagIds

`func (o *TaskInstancesBatchBody) GetDagIds() []string`

GetDagIds returns the DagIds field if non-nil, zero value otherwise.

### GetDagIdsOk

`func (o *TaskInstancesBatchBody) GetDagIdsOk() (*[]string, bool)`

GetDagIdsOk returns a tuple with the DagIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagIds

`func (o *TaskInstancesBatchBody) SetDagIds(v []string)`

SetDagIds sets DagIds field to given value.

### HasDagIds

`func (o *TaskInstancesBatchBody) HasDagIds() bool`

HasDagIds returns a boolean if a field has been set.

### GetDagRunIds

`func (o *TaskInstancesBatchBody) GetDagRunIds() []string`

GetDagRunIds returns the DagRunIds field if non-nil, zero value otherwise.

### GetDagRunIdsOk

`func (o *TaskInstancesBatchBody) GetDagRunIdsOk() (*[]string, bool)`

GetDagRunIdsOk returns a tuple with the DagRunIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagRunIds

`func (o *TaskInstancesBatchBody) SetDagRunIds(v []string)`

SetDagRunIds sets DagRunIds field to given value.

### HasDagRunIds

`func (o *TaskInstancesBatchBody) HasDagRunIds() bool`

HasDagRunIds returns a boolean if a field has been set.

### GetTaskIds

`func (o *TaskInstancesBatchBody) GetTaskIds() []string`

GetTaskIds returns the TaskIds field if non-nil, zero value otherwise.

### GetTaskIdsOk

`func (o *TaskInstancesBatchBody) GetTaskIdsOk() (*[]string, bool)`

GetTaskIdsOk returns a tuple with the TaskIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskIds

`func (o *TaskInstancesBatchBody) SetTaskIds(v []string)`

SetTaskIds sets TaskIds field to given value.

### HasTaskIds

`func (o *TaskInstancesBatchBody) HasTaskIds() bool`

HasTaskIds returns a boolean if a field has been set.

### GetState

`func (o *TaskInstancesBatchBody) GetState() []TaskInstanceState`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *TaskInstancesBatchBody) GetStateOk() (*[]TaskInstanceState, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *TaskInstancesBatchBody) SetState(v []TaskInstanceState)`

SetState sets State field to given value.

### HasState

`func (o *TaskInstancesBatchBody) HasState() bool`

HasState returns a boolean if a field has been set.

### GetRunAfterGte

`func (o *TaskInstancesBatchBody) GetRunAfterGte() time.Time`

GetRunAfterGte returns the RunAfterGte field if non-nil, zero value otherwise.

### GetRunAfterGteOk

`func (o *TaskInstancesBatchBody) GetRunAfterGteOk() (*time.Time, bool)`

GetRunAfterGteOk returns a tuple with the RunAfterGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfterGte

`func (o *TaskInstancesBatchBody) SetRunAfterGte(v time.Time)`

SetRunAfterGte sets RunAfterGte field to given value.

### HasRunAfterGte

`func (o *TaskInstancesBatchBody) HasRunAfterGte() bool`

HasRunAfterGte returns a boolean if a field has been set.

### GetRunAfterGt

`func (o *TaskInstancesBatchBody) GetRunAfterGt() time.Time`

GetRunAfterGt returns the RunAfterGt field if non-nil, zero value otherwise.

### GetRunAfterGtOk

`func (o *TaskInstancesBatchBody) GetRunAfterGtOk() (*time.Time, bool)`

GetRunAfterGtOk returns a tuple with the RunAfterGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfterGt

`func (o *TaskInstancesBatchBody) SetRunAfterGt(v time.Time)`

SetRunAfterGt sets RunAfterGt field to given value.

### HasRunAfterGt

`func (o *TaskInstancesBatchBody) HasRunAfterGt() bool`

HasRunAfterGt returns a boolean if a field has been set.

### GetRunAfterLte

`func (o *TaskInstancesBatchBody) GetRunAfterLte() time.Time`

GetRunAfterLte returns the RunAfterLte field if non-nil, zero value otherwise.

### GetRunAfterLteOk

`func (o *TaskInstancesBatchBody) GetRunAfterLteOk() (*time.Time, bool)`

GetRunAfterLteOk returns a tuple with the RunAfterLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfterLte

`func (o *TaskInstancesBatchBody) SetRunAfterLte(v time.Time)`

SetRunAfterLte sets RunAfterLte field to given value.

### HasRunAfterLte

`func (o *TaskInstancesBatchBody) HasRunAfterLte() bool`

HasRunAfterLte returns a boolean if a field has been set.

### GetRunAfterLt

`func (o *TaskInstancesBatchBody) GetRunAfterLt() time.Time`

GetRunAfterLt returns the RunAfterLt field if non-nil, zero value otherwise.

### GetRunAfterLtOk

`func (o *TaskInstancesBatchBody) GetRunAfterLtOk() (*time.Time, bool)`

GetRunAfterLtOk returns a tuple with the RunAfterLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfterLt

`func (o *TaskInstancesBatchBody) SetRunAfterLt(v time.Time)`

SetRunAfterLt sets RunAfterLt field to given value.

### HasRunAfterLt

`func (o *TaskInstancesBatchBody) HasRunAfterLt() bool`

HasRunAfterLt returns a boolean if a field has been set.

### GetLogicalDateGte

`func (o *TaskInstancesBatchBody) GetLogicalDateGte() time.Time`

GetLogicalDateGte returns the LogicalDateGte field if non-nil, zero value otherwise.

### GetLogicalDateGteOk

`func (o *TaskInstancesBatchBody) GetLogicalDateGteOk() (*time.Time, bool)`

GetLogicalDateGteOk returns a tuple with the LogicalDateGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDateGte

`func (o *TaskInstancesBatchBody) SetLogicalDateGte(v time.Time)`

SetLogicalDateGte sets LogicalDateGte field to given value.

### HasLogicalDateGte

`func (o *TaskInstancesBatchBody) HasLogicalDateGte() bool`

HasLogicalDateGte returns a boolean if a field has been set.

### GetLogicalDateGt

`func (o *TaskInstancesBatchBody) GetLogicalDateGt() time.Time`

GetLogicalDateGt returns the LogicalDateGt field if non-nil, zero value otherwise.

### GetLogicalDateGtOk

`func (o *TaskInstancesBatchBody) GetLogicalDateGtOk() (*time.Time, bool)`

GetLogicalDateGtOk returns a tuple with the LogicalDateGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDateGt

`func (o *TaskInstancesBatchBody) SetLogicalDateGt(v time.Time)`

SetLogicalDateGt sets LogicalDateGt field to given value.

### HasLogicalDateGt

`func (o *TaskInstancesBatchBody) HasLogicalDateGt() bool`

HasLogicalDateGt returns a boolean if a field has been set.

### GetLogicalDateLte

`func (o *TaskInstancesBatchBody) GetLogicalDateLte() time.Time`

GetLogicalDateLte returns the LogicalDateLte field if non-nil, zero value otherwise.

### GetLogicalDateLteOk

`func (o *TaskInstancesBatchBody) GetLogicalDateLteOk() (*time.Time, bool)`

GetLogicalDateLteOk returns a tuple with the LogicalDateLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDateLte

`func (o *TaskInstancesBatchBody) SetLogicalDateLte(v time.Time)`

SetLogicalDateLte sets LogicalDateLte field to given value.

### HasLogicalDateLte

`func (o *TaskInstancesBatchBody) HasLogicalDateLte() bool`

HasLogicalDateLte returns a boolean if a field has been set.

### GetLogicalDateLt

`func (o *TaskInstancesBatchBody) GetLogicalDateLt() time.Time`

GetLogicalDateLt returns the LogicalDateLt field if non-nil, zero value otherwise.

### GetLogicalDateLtOk

`func (o *TaskInstancesBatchBody) GetLogicalDateLtOk() (*time.Time, bool)`

GetLogicalDateLtOk returns a tuple with the LogicalDateLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDateLt

`func (o *TaskInstancesBatchBody) SetLogicalDateLt(v time.Time)`

SetLogicalDateLt sets LogicalDateLt field to given value.

### HasLogicalDateLt

`func (o *TaskInstancesBatchBody) HasLogicalDateLt() bool`

HasLogicalDateLt returns a boolean if a field has been set.

### GetStartDateGte

`func (o *TaskInstancesBatchBody) GetStartDateGte() time.Time`

GetStartDateGte returns the StartDateGte field if non-nil, zero value otherwise.

### GetStartDateGteOk

`func (o *TaskInstancesBatchBody) GetStartDateGteOk() (*time.Time, bool)`

GetStartDateGteOk returns a tuple with the StartDateGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDateGte

`func (o *TaskInstancesBatchBody) SetStartDateGte(v time.Time)`

SetStartDateGte sets StartDateGte field to given value.

### HasStartDateGte

`func (o *TaskInstancesBatchBody) HasStartDateGte() bool`

HasStartDateGte returns a boolean if a field has been set.

### GetStartDateGt

`func (o *TaskInstancesBatchBody) GetStartDateGt() time.Time`

GetStartDateGt returns the StartDateGt field if non-nil, zero value otherwise.

### GetStartDateGtOk

`func (o *TaskInstancesBatchBody) GetStartDateGtOk() (*time.Time, bool)`

GetStartDateGtOk returns a tuple with the StartDateGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDateGt

`func (o *TaskInstancesBatchBody) SetStartDateGt(v time.Time)`

SetStartDateGt sets StartDateGt field to given value.

### HasStartDateGt

`func (o *TaskInstancesBatchBody) HasStartDateGt() bool`

HasStartDateGt returns a boolean if a field has been set.

### GetStartDateLte

`func (o *TaskInstancesBatchBody) GetStartDateLte() time.Time`

GetStartDateLte returns the StartDateLte field if non-nil, zero value otherwise.

### GetStartDateLteOk

`func (o *TaskInstancesBatchBody) GetStartDateLteOk() (*time.Time, bool)`

GetStartDateLteOk returns a tuple with the StartDateLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDateLte

`func (o *TaskInstancesBatchBody) SetStartDateLte(v time.Time)`

SetStartDateLte sets StartDateLte field to given value.

### HasStartDateLte

`func (o *TaskInstancesBatchBody) HasStartDateLte() bool`

HasStartDateLte returns a boolean if a field has been set.

### GetStartDateLt

`func (o *TaskInstancesBatchBody) GetStartDateLt() time.Time`

GetStartDateLt returns the StartDateLt field if non-nil, zero value otherwise.

### GetStartDateLtOk

`func (o *TaskInstancesBatchBody) GetStartDateLtOk() (*time.Time, bool)`

GetStartDateLtOk returns a tuple with the StartDateLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDateLt

`func (o *TaskInstancesBatchBody) SetStartDateLt(v time.Time)`

SetStartDateLt sets StartDateLt field to given value.

### HasStartDateLt

`func (o *TaskInstancesBatchBody) HasStartDateLt() bool`

HasStartDateLt returns a boolean if a field has been set.

### GetEndDateGte

`func (o *TaskInstancesBatchBody) GetEndDateGte() time.Time`

GetEndDateGte returns the EndDateGte field if non-nil, zero value otherwise.

### GetEndDateGteOk

`func (o *TaskInstancesBatchBody) GetEndDateGteOk() (*time.Time, bool)`

GetEndDateGteOk returns a tuple with the EndDateGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDateGte

`func (o *TaskInstancesBatchBody) SetEndDateGte(v time.Time)`

SetEndDateGte sets EndDateGte field to given value.

### HasEndDateGte

`func (o *TaskInstancesBatchBody) HasEndDateGte() bool`

HasEndDateGte returns a boolean if a field has been set.

### GetEndDateGt

`func (o *TaskInstancesBatchBody) GetEndDateGt() time.Time`

GetEndDateGt returns the EndDateGt field if non-nil, zero value otherwise.

### GetEndDateGtOk

`func (o *TaskInstancesBatchBody) GetEndDateGtOk() (*time.Time, bool)`

GetEndDateGtOk returns a tuple with the EndDateGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDateGt

`func (o *TaskInstancesBatchBody) SetEndDateGt(v time.Time)`

SetEndDateGt sets EndDateGt field to given value.

### HasEndDateGt

`func (o *TaskInstancesBatchBody) HasEndDateGt() bool`

HasEndDateGt returns a boolean if a field has been set.

### GetEndDateLte

`func (o *TaskInstancesBatchBody) GetEndDateLte() time.Time`

GetEndDateLte returns the EndDateLte field if non-nil, zero value otherwise.

### GetEndDateLteOk

`func (o *TaskInstancesBatchBody) GetEndDateLteOk() (*time.Time, bool)`

GetEndDateLteOk returns a tuple with the EndDateLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDateLte

`func (o *TaskInstancesBatchBody) SetEndDateLte(v time.Time)`

SetEndDateLte sets EndDateLte field to given value.

### HasEndDateLte

`func (o *TaskInstancesBatchBody) HasEndDateLte() bool`

HasEndDateLte returns a boolean if a field has been set.

### GetEndDateLt

`func (o *TaskInstancesBatchBody) GetEndDateLt() time.Time`

GetEndDateLt returns the EndDateLt field if non-nil, zero value otherwise.

### GetEndDateLtOk

`func (o *TaskInstancesBatchBody) GetEndDateLtOk() (*time.Time, bool)`

GetEndDateLtOk returns a tuple with the EndDateLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDateLt

`func (o *TaskInstancesBatchBody) SetEndDateLt(v time.Time)`

SetEndDateLt sets EndDateLt field to given value.

### HasEndDateLt

`func (o *TaskInstancesBatchBody) HasEndDateLt() bool`

HasEndDateLt returns a boolean if a field has been set.

### GetDurationGte

`func (o *TaskInstancesBatchBody) GetDurationGte() float32`

GetDurationGte returns the DurationGte field if non-nil, zero value otherwise.

### GetDurationGteOk

`func (o *TaskInstancesBatchBody) GetDurationGteOk() (*float32, bool)`

GetDurationGteOk returns a tuple with the DurationGte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationGte

`func (o *TaskInstancesBatchBody) SetDurationGte(v float32)`

SetDurationGte sets DurationGte field to given value.

### HasDurationGte

`func (o *TaskInstancesBatchBody) HasDurationGte() bool`

HasDurationGte returns a boolean if a field has been set.

### GetDurationGt

`func (o *TaskInstancesBatchBody) GetDurationGt() float32`

GetDurationGt returns the DurationGt field if non-nil, zero value otherwise.

### GetDurationGtOk

`func (o *TaskInstancesBatchBody) GetDurationGtOk() (*float32, bool)`

GetDurationGtOk returns a tuple with the DurationGt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationGt

`func (o *TaskInstancesBatchBody) SetDurationGt(v float32)`

SetDurationGt sets DurationGt field to given value.

### HasDurationGt

`func (o *TaskInstancesBatchBody) HasDurationGt() bool`

HasDurationGt returns a boolean if a field has been set.

### GetDurationLte

`func (o *TaskInstancesBatchBody) GetDurationLte() float32`

GetDurationLte returns the DurationLte field if non-nil, zero value otherwise.

### GetDurationLteOk

`func (o *TaskInstancesBatchBody) GetDurationLteOk() (*float32, bool)`

GetDurationLteOk returns a tuple with the DurationLte field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationLte

`func (o *TaskInstancesBatchBody) SetDurationLte(v float32)`

SetDurationLte sets DurationLte field to given value.

### HasDurationLte

`func (o *TaskInstancesBatchBody) HasDurationLte() bool`

HasDurationLte returns a boolean if a field has been set.

### GetDurationLt

`func (o *TaskInstancesBatchBody) GetDurationLt() float32`

GetDurationLt returns the DurationLt field if non-nil, zero value otherwise.

### GetDurationLtOk

`func (o *TaskInstancesBatchBody) GetDurationLtOk() (*float32, bool)`

GetDurationLtOk returns a tuple with the DurationLt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationLt

`func (o *TaskInstancesBatchBody) SetDurationLt(v float32)`

SetDurationLt sets DurationLt field to given value.

### HasDurationLt

`func (o *TaskInstancesBatchBody) HasDurationLt() bool`

HasDurationLt returns a boolean if a field has been set.

### GetPool

`func (o *TaskInstancesBatchBody) GetPool() []string`

GetPool returns the Pool field if non-nil, zero value otherwise.

### GetPoolOk

`func (o *TaskInstancesBatchBody) GetPoolOk() (*[]string, bool)`

GetPoolOk returns a tuple with the Pool field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPool

`func (o *TaskInstancesBatchBody) SetPool(v []string)`

SetPool sets Pool field to given value.

### HasPool

`func (o *TaskInstancesBatchBody) HasPool() bool`

HasPool returns a boolean if a field has been set.

### GetQueue

`func (o *TaskInstancesBatchBody) GetQueue() []string`

GetQueue returns the Queue field if non-nil, zero value otherwise.

### GetQueueOk

`func (o *TaskInstancesBatchBody) GetQueueOk() (*[]string, bool)`

GetQueueOk returns a tuple with the Queue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueue

`func (o *TaskInstancesBatchBody) SetQueue(v []string)`

SetQueue sets Queue field to given value.

### HasQueue

`func (o *TaskInstancesBatchBody) HasQueue() bool`

HasQueue returns a boolean if a field has been set.

### GetExecutor

`func (o *TaskInstancesBatchBody) GetExecutor() []string`

GetExecutor returns the Executor field if non-nil, zero value otherwise.

### GetExecutorOk

`func (o *TaskInstancesBatchBody) GetExecutorOk() (*[]string, bool)`

GetExecutorOk returns a tuple with the Executor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutor

`func (o *TaskInstancesBatchBody) SetExecutor(v []string)`

SetExecutor sets Executor field to given value.

### HasExecutor

`func (o *TaskInstancesBatchBody) HasExecutor() bool`

HasExecutor returns a boolean if a field has been set.

### GetPageOffset

`func (o *TaskInstancesBatchBody) GetPageOffset() int32`

GetPageOffset returns the PageOffset field if non-nil, zero value otherwise.

### GetPageOffsetOk

`func (o *TaskInstancesBatchBody) GetPageOffsetOk() (*int32, bool)`

GetPageOffsetOk returns a tuple with the PageOffset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageOffset

`func (o *TaskInstancesBatchBody) SetPageOffset(v int32)`

SetPageOffset sets PageOffset field to given value.

### HasPageOffset

`func (o *TaskInstancesBatchBody) HasPageOffset() bool`

HasPageOffset returns a boolean if a field has been set.

### GetPageLimit

`func (o *TaskInstancesBatchBody) GetPageLimit() int32`

GetPageLimit returns the PageLimit field if non-nil, zero value otherwise.

### GetPageLimitOk

`func (o *TaskInstancesBatchBody) GetPageLimitOk() (*int32, bool)`

GetPageLimitOk returns a tuple with the PageLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPageLimit

`func (o *TaskInstancesBatchBody) SetPageLimit(v int32)`

SetPageLimit sets PageLimit field to given value.

### HasPageLimit

`func (o *TaskInstancesBatchBody) HasPageLimit() bool`

HasPageLimit returns a boolean if a field has been set.

### GetOrderBy

`func (o *TaskInstancesBatchBody) GetOrderBy() string`

GetOrderBy returns the OrderBy field if non-nil, zero value otherwise.

### GetOrderByOk

`func (o *TaskInstancesBatchBody) GetOrderByOk() (*string, bool)`

GetOrderByOk returns a tuple with the OrderBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrderBy

`func (o *TaskInstancesBatchBody) SetOrderBy(v string)`

SetOrderBy sets OrderBy field to given value.

### HasOrderBy

`func (o *TaskInstancesBatchBody) HasOrderBy() bool`

HasOrderBy returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


