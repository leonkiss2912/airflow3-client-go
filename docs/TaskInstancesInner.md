# TaskInstancesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**TaskId** | **string** |  | 
**DagId** | **string** |  | 
**DagRunId** | **string** |  | 
**MapIndex** | **int32** |  | 
**LogicalDate** | **time.Time** |  | 
**RunAfter** | **time.Time** |  | 
**StartDate** | **time.Time** |  | 
**EndDate** | **time.Time** |  | 
**Duration** | **float32** |  | 
**State** | [**TaskInstanceState**](TaskInstanceState.md) |  | 
**TryNumber** | **int32** |  | 
**MaxTries** | **int32** |  | 
**TaskDisplayName** | **string** |  | 
**DagDisplayName** | **string** |  | 
**Hostname** | **string** |  | 
**Unixname** | **string** |  | 
**Pool** | **string** |  | 
**PoolSlots** | **int32** |  | 
**Queue** | **string** |  | 
**PriorityWeight** | **int32** |  | 
**Operator** | **string** |  | 
**OperatorName** | **string** |  | 
**QueuedWhen** | **time.Time** |  | 
**ScheduledWhen** | **time.Time** |  | 
**Pid** | **int32** |  | 
**Executor** | **string** |  | 
**ExecutorConfig** | **string** |  | 
**Note** | **string** |  | 
**RenderedMapIndex** | **string** |  | 
**RenderedFields** | Pointer to **map[string]interface{}** |  | [optional] 
**Trigger** | [**TriggerResponse**](TriggerResponse.md) |  | 
**TriggererJob** | [**JobResponse**](JobResponse.md) |  | 
**DagVersion** | [**DagVersionResponse**](DagVersionResponse.md) |  | 

## Methods

### NewTaskInstancesInner

`func NewTaskInstancesInner(id string, taskId string, dagId string, dagRunId string, mapIndex int32, logicalDate time.Time, runAfter time.Time, startDate time.Time, endDate time.Time, duration float32, state TaskInstanceState, tryNumber int32, maxTries int32, taskDisplayName string, dagDisplayName string, hostname string, unixname string, pool string, poolSlots int32, queue string, priorityWeight int32, operator string, operatorName string, queuedWhen time.Time, scheduledWhen time.Time, pid int32, executor string, executorConfig string, note string, renderedMapIndex string, trigger TriggerResponse, triggererJob JobResponse, dagVersion DagVersionResponse, ) *TaskInstancesInner`

NewTaskInstancesInner instantiates a new TaskInstancesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaskInstancesInnerWithDefaults

`func NewTaskInstancesInnerWithDefaults() *TaskInstancesInner`

NewTaskInstancesInnerWithDefaults instantiates a new TaskInstancesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *TaskInstancesInner) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *TaskInstancesInner) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *TaskInstancesInner) SetId(v string)`

SetId sets Id field to given value.


### GetTaskId

`func (o *TaskInstancesInner) GetTaskId() string`

GetTaskId returns the TaskId field if non-nil, zero value otherwise.

### GetTaskIdOk

`func (o *TaskInstancesInner) GetTaskIdOk() (*string, bool)`

GetTaskIdOk returns a tuple with the TaskId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskId

`func (o *TaskInstancesInner) SetTaskId(v string)`

SetTaskId sets TaskId field to given value.


### GetDagId

`func (o *TaskInstancesInner) GetDagId() string`

GetDagId returns the DagId field if non-nil, zero value otherwise.

### GetDagIdOk

`func (o *TaskInstancesInner) GetDagIdOk() (*string, bool)`

GetDagIdOk returns a tuple with the DagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagId

`func (o *TaskInstancesInner) SetDagId(v string)`

SetDagId sets DagId field to given value.


### GetDagRunId

`func (o *TaskInstancesInner) GetDagRunId() string`

GetDagRunId returns the DagRunId field if non-nil, zero value otherwise.

### GetDagRunIdOk

`func (o *TaskInstancesInner) GetDagRunIdOk() (*string, bool)`

GetDagRunIdOk returns a tuple with the DagRunId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagRunId

`func (o *TaskInstancesInner) SetDagRunId(v string)`

SetDagRunId sets DagRunId field to given value.


### GetMapIndex

`func (o *TaskInstancesInner) GetMapIndex() int32`

GetMapIndex returns the MapIndex field if non-nil, zero value otherwise.

### GetMapIndexOk

`func (o *TaskInstancesInner) GetMapIndexOk() (*int32, bool)`

GetMapIndexOk returns a tuple with the MapIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMapIndex

`func (o *TaskInstancesInner) SetMapIndex(v int32)`

SetMapIndex sets MapIndex field to given value.


### GetLogicalDate

`func (o *TaskInstancesInner) GetLogicalDate() time.Time`

GetLogicalDate returns the LogicalDate field if non-nil, zero value otherwise.

### GetLogicalDateOk

`func (o *TaskInstancesInner) GetLogicalDateOk() (*time.Time, bool)`

GetLogicalDateOk returns a tuple with the LogicalDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDate

`func (o *TaskInstancesInner) SetLogicalDate(v time.Time)`

SetLogicalDate sets LogicalDate field to given value.


### GetRunAfter

`func (o *TaskInstancesInner) GetRunAfter() time.Time`

GetRunAfter returns the RunAfter field if non-nil, zero value otherwise.

### GetRunAfterOk

`func (o *TaskInstancesInner) GetRunAfterOk() (*time.Time, bool)`

GetRunAfterOk returns a tuple with the RunAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfter

`func (o *TaskInstancesInner) SetRunAfter(v time.Time)`

SetRunAfter sets RunAfter field to given value.


### GetStartDate

`func (o *TaskInstancesInner) GetStartDate() time.Time`

GetStartDate returns the StartDate field if non-nil, zero value otherwise.

### GetStartDateOk

`func (o *TaskInstancesInner) GetStartDateOk() (*time.Time, bool)`

GetStartDateOk returns a tuple with the StartDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDate

`func (o *TaskInstancesInner) SetStartDate(v time.Time)`

SetStartDate sets StartDate field to given value.


### GetEndDate

`func (o *TaskInstancesInner) GetEndDate() time.Time`

GetEndDate returns the EndDate field if non-nil, zero value otherwise.

### GetEndDateOk

`func (o *TaskInstancesInner) GetEndDateOk() (*time.Time, bool)`

GetEndDateOk returns a tuple with the EndDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDate

`func (o *TaskInstancesInner) SetEndDate(v time.Time)`

SetEndDate sets EndDate field to given value.


### GetDuration

`func (o *TaskInstancesInner) GetDuration() float32`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *TaskInstancesInner) GetDurationOk() (*float32, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *TaskInstancesInner) SetDuration(v float32)`

SetDuration sets Duration field to given value.


### GetState

`func (o *TaskInstancesInner) GetState() TaskInstanceState`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *TaskInstancesInner) GetStateOk() (*TaskInstanceState, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *TaskInstancesInner) SetState(v TaskInstanceState)`

SetState sets State field to given value.


### GetTryNumber

`func (o *TaskInstancesInner) GetTryNumber() int32`

GetTryNumber returns the TryNumber field if non-nil, zero value otherwise.

### GetTryNumberOk

`func (o *TaskInstancesInner) GetTryNumberOk() (*int32, bool)`

GetTryNumberOk returns a tuple with the TryNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTryNumber

`func (o *TaskInstancesInner) SetTryNumber(v int32)`

SetTryNumber sets TryNumber field to given value.


### GetMaxTries

`func (o *TaskInstancesInner) GetMaxTries() int32`

GetMaxTries returns the MaxTries field if non-nil, zero value otherwise.

### GetMaxTriesOk

`func (o *TaskInstancesInner) GetMaxTriesOk() (*int32, bool)`

GetMaxTriesOk returns a tuple with the MaxTries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxTries

`func (o *TaskInstancesInner) SetMaxTries(v int32)`

SetMaxTries sets MaxTries field to given value.


### GetTaskDisplayName

`func (o *TaskInstancesInner) GetTaskDisplayName() string`

GetTaskDisplayName returns the TaskDisplayName field if non-nil, zero value otherwise.

### GetTaskDisplayNameOk

`func (o *TaskInstancesInner) GetTaskDisplayNameOk() (*string, bool)`

GetTaskDisplayNameOk returns a tuple with the TaskDisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskDisplayName

`func (o *TaskInstancesInner) SetTaskDisplayName(v string)`

SetTaskDisplayName sets TaskDisplayName field to given value.


### GetDagDisplayName

`func (o *TaskInstancesInner) GetDagDisplayName() string`

GetDagDisplayName returns the DagDisplayName field if non-nil, zero value otherwise.

### GetDagDisplayNameOk

`func (o *TaskInstancesInner) GetDagDisplayNameOk() (*string, bool)`

GetDagDisplayNameOk returns a tuple with the DagDisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagDisplayName

`func (o *TaskInstancesInner) SetDagDisplayName(v string)`

SetDagDisplayName sets DagDisplayName field to given value.


### GetHostname

`func (o *TaskInstancesInner) GetHostname() string`

GetHostname returns the Hostname field if non-nil, zero value otherwise.

### GetHostnameOk

`func (o *TaskInstancesInner) GetHostnameOk() (*string, bool)`

GetHostnameOk returns a tuple with the Hostname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostname

`func (o *TaskInstancesInner) SetHostname(v string)`

SetHostname sets Hostname field to given value.


### GetUnixname

`func (o *TaskInstancesInner) GetUnixname() string`

GetUnixname returns the Unixname field if non-nil, zero value otherwise.

### GetUnixnameOk

`func (o *TaskInstancesInner) GetUnixnameOk() (*string, bool)`

GetUnixnameOk returns a tuple with the Unixname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnixname

`func (o *TaskInstancesInner) SetUnixname(v string)`

SetUnixname sets Unixname field to given value.


### GetPool

`func (o *TaskInstancesInner) GetPool() string`

GetPool returns the Pool field if non-nil, zero value otherwise.

### GetPoolOk

`func (o *TaskInstancesInner) GetPoolOk() (*string, bool)`

GetPoolOk returns a tuple with the Pool field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPool

`func (o *TaskInstancesInner) SetPool(v string)`

SetPool sets Pool field to given value.


### GetPoolSlots

`func (o *TaskInstancesInner) GetPoolSlots() int32`

GetPoolSlots returns the PoolSlots field if non-nil, zero value otherwise.

### GetPoolSlotsOk

`func (o *TaskInstancesInner) GetPoolSlotsOk() (*int32, bool)`

GetPoolSlotsOk returns a tuple with the PoolSlots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPoolSlots

`func (o *TaskInstancesInner) SetPoolSlots(v int32)`

SetPoolSlots sets PoolSlots field to given value.


### GetQueue

`func (o *TaskInstancesInner) GetQueue() string`

GetQueue returns the Queue field if non-nil, zero value otherwise.

### GetQueueOk

`func (o *TaskInstancesInner) GetQueueOk() (*string, bool)`

GetQueueOk returns a tuple with the Queue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueue

`func (o *TaskInstancesInner) SetQueue(v string)`

SetQueue sets Queue field to given value.


### GetPriorityWeight

`func (o *TaskInstancesInner) GetPriorityWeight() int32`

GetPriorityWeight returns the PriorityWeight field if non-nil, zero value otherwise.

### GetPriorityWeightOk

`func (o *TaskInstancesInner) GetPriorityWeightOk() (*int32, bool)`

GetPriorityWeightOk returns a tuple with the PriorityWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriorityWeight

`func (o *TaskInstancesInner) SetPriorityWeight(v int32)`

SetPriorityWeight sets PriorityWeight field to given value.


### GetOperator

`func (o *TaskInstancesInner) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *TaskInstancesInner) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *TaskInstancesInner) SetOperator(v string)`

SetOperator sets Operator field to given value.


### GetOperatorName

`func (o *TaskInstancesInner) GetOperatorName() string`

GetOperatorName returns the OperatorName field if non-nil, zero value otherwise.

### GetOperatorNameOk

`func (o *TaskInstancesInner) GetOperatorNameOk() (*string, bool)`

GetOperatorNameOk returns a tuple with the OperatorName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperatorName

`func (o *TaskInstancesInner) SetOperatorName(v string)`

SetOperatorName sets OperatorName field to given value.


### GetQueuedWhen

`func (o *TaskInstancesInner) GetQueuedWhen() time.Time`

GetQueuedWhen returns the QueuedWhen field if non-nil, zero value otherwise.

### GetQueuedWhenOk

`func (o *TaskInstancesInner) GetQueuedWhenOk() (*time.Time, bool)`

GetQueuedWhenOk returns a tuple with the QueuedWhen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedWhen

`func (o *TaskInstancesInner) SetQueuedWhen(v time.Time)`

SetQueuedWhen sets QueuedWhen field to given value.


### GetScheduledWhen

`func (o *TaskInstancesInner) GetScheduledWhen() time.Time`

GetScheduledWhen returns the ScheduledWhen field if non-nil, zero value otherwise.

### GetScheduledWhenOk

`func (o *TaskInstancesInner) GetScheduledWhenOk() (*time.Time, bool)`

GetScheduledWhenOk returns a tuple with the ScheduledWhen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScheduledWhen

`func (o *TaskInstancesInner) SetScheduledWhen(v time.Time)`

SetScheduledWhen sets ScheduledWhen field to given value.


### GetPid

`func (o *TaskInstancesInner) GetPid() int32`

GetPid returns the Pid field if non-nil, zero value otherwise.

### GetPidOk

`func (o *TaskInstancesInner) GetPidOk() (*int32, bool)`

GetPidOk returns a tuple with the Pid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPid

`func (o *TaskInstancesInner) SetPid(v int32)`

SetPid sets Pid field to given value.


### GetExecutor

`func (o *TaskInstancesInner) GetExecutor() string`

GetExecutor returns the Executor field if non-nil, zero value otherwise.

### GetExecutorOk

`func (o *TaskInstancesInner) GetExecutorOk() (*string, bool)`

GetExecutorOk returns a tuple with the Executor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutor

`func (o *TaskInstancesInner) SetExecutor(v string)`

SetExecutor sets Executor field to given value.


### GetExecutorConfig

`func (o *TaskInstancesInner) GetExecutorConfig() string`

GetExecutorConfig returns the ExecutorConfig field if non-nil, zero value otherwise.

### GetExecutorConfigOk

`func (o *TaskInstancesInner) GetExecutorConfigOk() (*string, bool)`

GetExecutorConfigOk returns a tuple with the ExecutorConfig field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutorConfig

`func (o *TaskInstancesInner) SetExecutorConfig(v string)`

SetExecutorConfig sets ExecutorConfig field to given value.


### GetNote

`func (o *TaskInstancesInner) GetNote() string`

GetNote returns the Note field if non-nil, zero value otherwise.

### GetNoteOk

`func (o *TaskInstancesInner) GetNoteOk() (*string, bool)`

GetNoteOk returns a tuple with the Note field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNote

`func (o *TaskInstancesInner) SetNote(v string)`

SetNote sets Note field to given value.


### GetRenderedMapIndex

`func (o *TaskInstancesInner) GetRenderedMapIndex() string`

GetRenderedMapIndex returns the RenderedMapIndex field if non-nil, zero value otherwise.

### GetRenderedMapIndexOk

`func (o *TaskInstancesInner) GetRenderedMapIndexOk() (*string, bool)`

GetRenderedMapIndexOk returns a tuple with the RenderedMapIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenderedMapIndex

`func (o *TaskInstancesInner) SetRenderedMapIndex(v string)`

SetRenderedMapIndex sets RenderedMapIndex field to given value.


### GetRenderedFields

`func (o *TaskInstancesInner) GetRenderedFields() map[string]interface{}`

GetRenderedFields returns the RenderedFields field if non-nil, zero value otherwise.

### GetRenderedFieldsOk

`func (o *TaskInstancesInner) GetRenderedFieldsOk() (*map[string]interface{}, bool)`

GetRenderedFieldsOk returns a tuple with the RenderedFields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRenderedFields

`func (o *TaskInstancesInner) SetRenderedFields(v map[string]interface{})`

SetRenderedFields sets RenderedFields field to given value.

### HasRenderedFields

`func (o *TaskInstancesInner) HasRenderedFields() bool`

HasRenderedFields returns a boolean if a field has been set.

### GetTrigger

`func (o *TaskInstancesInner) GetTrigger() TriggerResponse`

GetTrigger returns the Trigger field if non-nil, zero value otherwise.

### GetTriggerOk

`func (o *TaskInstancesInner) GetTriggerOk() (*TriggerResponse, bool)`

GetTriggerOk returns a tuple with the Trigger field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrigger

`func (o *TaskInstancesInner) SetTrigger(v TriggerResponse)`

SetTrigger sets Trigger field to given value.


### GetTriggererJob

`func (o *TaskInstancesInner) GetTriggererJob() JobResponse`

GetTriggererJob returns the TriggererJob field if non-nil, zero value otherwise.

### GetTriggererJobOk

`func (o *TaskInstancesInner) GetTriggererJobOk() (*JobResponse, bool)`

GetTriggererJobOk returns a tuple with the TriggererJob field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTriggererJob

`func (o *TaskInstancesInner) SetTriggererJob(v JobResponse)`

SetTriggererJob sets TriggererJob field to given value.


### GetDagVersion

`func (o *TaskInstancesInner) GetDagVersion() DagVersionResponse`

GetDagVersion returns the DagVersion field if non-nil, zero value otherwise.

### GetDagVersionOk

`func (o *TaskInstancesInner) GetDagVersionOk() (*DagVersionResponse, bool)`

GetDagVersionOk returns a tuple with the DagVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagVersion

`func (o *TaskInstancesInner) SetDagVersion(v DagVersionResponse)`

SetDagVersion sets DagVersion field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


