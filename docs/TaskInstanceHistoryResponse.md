# TaskInstanceHistoryResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TaskId** | **string** |  | 
**DagId** | **string** |  | 
**DagRunId** | **string** |  | 
**MapIndex** | **int32** |  | 
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
**DagVersion** | [**DagVersionResponse**](DagVersionResponse.md) |  | 

## Methods

### NewTaskInstanceHistoryResponse

`func NewTaskInstanceHistoryResponse(taskId string, dagId string, dagRunId string, mapIndex int32, startDate time.Time, endDate time.Time, duration float32, state TaskInstanceState, tryNumber int32, maxTries int32, taskDisplayName string, dagDisplayName string, hostname string, unixname string, pool string, poolSlots int32, queue string, priorityWeight int32, operator string, operatorName string, queuedWhen time.Time, scheduledWhen time.Time, pid int32, executor string, executorConfig string, dagVersion DagVersionResponse, ) *TaskInstanceHistoryResponse`

NewTaskInstanceHistoryResponse instantiates a new TaskInstanceHistoryResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaskInstanceHistoryResponseWithDefaults

`func NewTaskInstanceHistoryResponseWithDefaults() *TaskInstanceHistoryResponse`

NewTaskInstanceHistoryResponseWithDefaults instantiates a new TaskInstanceHistoryResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTaskId

`func (o *TaskInstanceHistoryResponse) GetTaskId() string`

GetTaskId returns the TaskId field if non-nil, zero value otherwise.

### GetTaskIdOk

`func (o *TaskInstanceHistoryResponse) GetTaskIdOk() (*string, bool)`

GetTaskIdOk returns a tuple with the TaskId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskId

`func (o *TaskInstanceHistoryResponse) SetTaskId(v string)`

SetTaskId sets TaskId field to given value.


### GetDagId

`func (o *TaskInstanceHistoryResponse) GetDagId() string`

GetDagId returns the DagId field if non-nil, zero value otherwise.

### GetDagIdOk

`func (o *TaskInstanceHistoryResponse) GetDagIdOk() (*string, bool)`

GetDagIdOk returns a tuple with the DagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagId

`func (o *TaskInstanceHistoryResponse) SetDagId(v string)`

SetDagId sets DagId field to given value.


### GetDagRunId

`func (o *TaskInstanceHistoryResponse) GetDagRunId() string`

GetDagRunId returns the DagRunId field if non-nil, zero value otherwise.

### GetDagRunIdOk

`func (o *TaskInstanceHistoryResponse) GetDagRunIdOk() (*string, bool)`

GetDagRunIdOk returns a tuple with the DagRunId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagRunId

`func (o *TaskInstanceHistoryResponse) SetDagRunId(v string)`

SetDagRunId sets DagRunId field to given value.


### GetMapIndex

`func (o *TaskInstanceHistoryResponse) GetMapIndex() int32`

GetMapIndex returns the MapIndex field if non-nil, zero value otherwise.

### GetMapIndexOk

`func (o *TaskInstanceHistoryResponse) GetMapIndexOk() (*int32, bool)`

GetMapIndexOk returns a tuple with the MapIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMapIndex

`func (o *TaskInstanceHistoryResponse) SetMapIndex(v int32)`

SetMapIndex sets MapIndex field to given value.


### GetStartDate

`func (o *TaskInstanceHistoryResponse) GetStartDate() time.Time`

GetStartDate returns the StartDate field if non-nil, zero value otherwise.

### GetStartDateOk

`func (o *TaskInstanceHistoryResponse) GetStartDateOk() (*time.Time, bool)`

GetStartDateOk returns a tuple with the StartDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDate

`func (o *TaskInstanceHistoryResponse) SetStartDate(v time.Time)`

SetStartDate sets StartDate field to given value.


### GetEndDate

`func (o *TaskInstanceHistoryResponse) GetEndDate() time.Time`

GetEndDate returns the EndDate field if non-nil, zero value otherwise.

### GetEndDateOk

`func (o *TaskInstanceHistoryResponse) GetEndDateOk() (*time.Time, bool)`

GetEndDateOk returns a tuple with the EndDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDate

`func (o *TaskInstanceHistoryResponse) SetEndDate(v time.Time)`

SetEndDate sets EndDate field to given value.


### GetDuration

`func (o *TaskInstanceHistoryResponse) GetDuration() float32`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *TaskInstanceHistoryResponse) GetDurationOk() (*float32, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *TaskInstanceHistoryResponse) SetDuration(v float32)`

SetDuration sets Duration field to given value.


### GetState

`func (o *TaskInstanceHistoryResponse) GetState() TaskInstanceState`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *TaskInstanceHistoryResponse) GetStateOk() (*TaskInstanceState, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *TaskInstanceHistoryResponse) SetState(v TaskInstanceState)`

SetState sets State field to given value.


### GetTryNumber

`func (o *TaskInstanceHistoryResponse) GetTryNumber() int32`

GetTryNumber returns the TryNumber field if non-nil, zero value otherwise.

### GetTryNumberOk

`func (o *TaskInstanceHistoryResponse) GetTryNumberOk() (*int32, bool)`

GetTryNumberOk returns a tuple with the TryNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTryNumber

`func (o *TaskInstanceHistoryResponse) SetTryNumber(v int32)`

SetTryNumber sets TryNumber field to given value.


### GetMaxTries

`func (o *TaskInstanceHistoryResponse) GetMaxTries() int32`

GetMaxTries returns the MaxTries field if non-nil, zero value otherwise.

### GetMaxTriesOk

`func (o *TaskInstanceHistoryResponse) GetMaxTriesOk() (*int32, bool)`

GetMaxTriesOk returns a tuple with the MaxTries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxTries

`func (o *TaskInstanceHistoryResponse) SetMaxTries(v int32)`

SetMaxTries sets MaxTries field to given value.


### GetTaskDisplayName

`func (o *TaskInstanceHistoryResponse) GetTaskDisplayName() string`

GetTaskDisplayName returns the TaskDisplayName field if non-nil, zero value otherwise.

### GetTaskDisplayNameOk

`func (o *TaskInstanceHistoryResponse) GetTaskDisplayNameOk() (*string, bool)`

GetTaskDisplayNameOk returns a tuple with the TaskDisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskDisplayName

`func (o *TaskInstanceHistoryResponse) SetTaskDisplayName(v string)`

SetTaskDisplayName sets TaskDisplayName field to given value.


### GetDagDisplayName

`func (o *TaskInstanceHistoryResponse) GetDagDisplayName() string`

GetDagDisplayName returns the DagDisplayName field if non-nil, zero value otherwise.

### GetDagDisplayNameOk

`func (o *TaskInstanceHistoryResponse) GetDagDisplayNameOk() (*string, bool)`

GetDagDisplayNameOk returns a tuple with the DagDisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagDisplayName

`func (o *TaskInstanceHistoryResponse) SetDagDisplayName(v string)`

SetDagDisplayName sets DagDisplayName field to given value.


### GetHostname

`func (o *TaskInstanceHistoryResponse) GetHostname() string`

GetHostname returns the Hostname field if non-nil, zero value otherwise.

### GetHostnameOk

`func (o *TaskInstanceHistoryResponse) GetHostnameOk() (*string, bool)`

GetHostnameOk returns a tuple with the Hostname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostname

`func (o *TaskInstanceHistoryResponse) SetHostname(v string)`

SetHostname sets Hostname field to given value.


### GetUnixname

`func (o *TaskInstanceHistoryResponse) GetUnixname() string`

GetUnixname returns the Unixname field if non-nil, zero value otherwise.

### GetUnixnameOk

`func (o *TaskInstanceHistoryResponse) GetUnixnameOk() (*string, bool)`

GetUnixnameOk returns a tuple with the Unixname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnixname

`func (o *TaskInstanceHistoryResponse) SetUnixname(v string)`

SetUnixname sets Unixname field to given value.


### GetPool

`func (o *TaskInstanceHistoryResponse) GetPool() string`

GetPool returns the Pool field if non-nil, zero value otherwise.

### GetPoolOk

`func (o *TaskInstanceHistoryResponse) GetPoolOk() (*string, bool)`

GetPoolOk returns a tuple with the Pool field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPool

`func (o *TaskInstanceHistoryResponse) SetPool(v string)`

SetPool sets Pool field to given value.


### GetPoolSlots

`func (o *TaskInstanceHistoryResponse) GetPoolSlots() int32`

GetPoolSlots returns the PoolSlots field if non-nil, zero value otherwise.

### GetPoolSlotsOk

`func (o *TaskInstanceHistoryResponse) GetPoolSlotsOk() (*int32, bool)`

GetPoolSlotsOk returns a tuple with the PoolSlots field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPoolSlots

`func (o *TaskInstanceHistoryResponse) SetPoolSlots(v int32)`

SetPoolSlots sets PoolSlots field to given value.


### GetQueue

`func (o *TaskInstanceHistoryResponse) GetQueue() string`

GetQueue returns the Queue field if non-nil, zero value otherwise.

### GetQueueOk

`func (o *TaskInstanceHistoryResponse) GetQueueOk() (*string, bool)`

GetQueueOk returns a tuple with the Queue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueue

`func (o *TaskInstanceHistoryResponse) SetQueue(v string)`

SetQueue sets Queue field to given value.


### GetPriorityWeight

`func (o *TaskInstanceHistoryResponse) GetPriorityWeight() int32`

GetPriorityWeight returns the PriorityWeight field if non-nil, zero value otherwise.

### GetPriorityWeightOk

`func (o *TaskInstanceHistoryResponse) GetPriorityWeightOk() (*int32, bool)`

GetPriorityWeightOk returns a tuple with the PriorityWeight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriorityWeight

`func (o *TaskInstanceHistoryResponse) SetPriorityWeight(v int32)`

SetPriorityWeight sets PriorityWeight field to given value.


### GetOperator

`func (o *TaskInstanceHistoryResponse) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *TaskInstanceHistoryResponse) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *TaskInstanceHistoryResponse) SetOperator(v string)`

SetOperator sets Operator field to given value.


### GetOperatorName

`func (o *TaskInstanceHistoryResponse) GetOperatorName() string`

GetOperatorName returns the OperatorName field if non-nil, zero value otherwise.

### GetOperatorNameOk

`func (o *TaskInstanceHistoryResponse) GetOperatorNameOk() (*string, bool)`

GetOperatorNameOk returns a tuple with the OperatorName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperatorName

`func (o *TaskInstanceHistoryResponse) SetOperatorName(v string)`

SetOperatorName sets OperatorName field to given value.


### GetQueuedWhen

`func (o *TaskInstanceHistoryResponse) GetQueuedWhen() time.Time`

GetQueuedWhen returns the QueuedWhen field if non-nil, zero value otherwise.

### GetQueuedWhenOk

`func (o *TaskInstanceHistoryResponse) GetQueuedWhenOk() (*time.Time, bool)`

GetQueuedWhenOk returns a tuple with the QueuedWhen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedWhen

`func (o *TaskInstanceHistoryResponse) SetQueuedWhen(v time.Time)`

SetQueuedWhen sets QueuedWhen field to given value.


### GetScheduledWhen

`func (o *TaskInstanceHistoryResponse) GetScheduledWhen() time.Time`

GetScheduledWhen returns the ScheduledWhen field if non-nil, zero value otherwise.

### GetScheduledWhenOk

`func (o *TaskInstanceHistoryResponse) GetScheduledWhenOk() (*time.Time, bool)`

GetScheduledWhenOk returns a tuple with the ScheduledWhen field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScheduledWhen

`func (o *TaskInstanceHistoryResponse) SetScheduledWhen(v time.Time)`

SetScheduledWhen sets ScheduledWhen field to given value.


### GetPid

`func (o *TaskInstanceHistoryResponse) GetPid() int32`

GetPid returns the Pid field if non-nil, zero value otherwise.

### GetPidOk

`func (o *TaskInstanceHistoryResponse) GetPidOk() (*int32, bool)`

GetPidOk returns a tuple with the Pid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPid

`func (o *TaskInstanceHistoryResponse) SetPid(v int32)`

SetPid sets Pid field to given value.


### GetExecutor

`func (o *TaskInstanceHistoryResponse) GetExecutor() string`

GetExecutor returns the Executor field if non-nil, zero value otherwise.

### GetExecutorOk

`func (o *TaskInstanceHistoryResponse) GetExecutorOk() (*string, bool)`

GetExecutorOk returns a tuple with the Executor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutor

`func (o *TaskInstanceHistoryResponse) SetExecutor(v string)`

SetExecutor sets Executor field to given value.


### GetExecutorConfig

`func (o *TaskInstanceHistoryResponse) GetExecutorConfig() string`

GetExecutorConfig returns the ExecutorConfig field if non-nil, zero value otherwise.

### GetExecutorConfigOk

`func (o *TaskInstanceHistoryResponse) GetExecutorConfigOk() (*string, bool)`

GetExecutorConfigOk returns a tuple with the ExecutorConfig field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutorConfig

`func (o *TaskInstanceHistoryResponse) SetExecutorConfig(v string)`

SetExecutorConfig sets ExecutorConfig field to given value.


### GetDagVersion

`func (o *TaskInstanceHistoryResponse) GetDagVersion() DagVersionResponse`

GetDagVersion returns the DagVersion field if non-nil, zero value otherwise.

### GetDagVersionOk

`func (o *TaskInstanceHistoryResponse) GetDagVersionOk() (*DagVersionResponse, bool)`

GetDagVersionOk returns a tuple with the DagVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagVersion

`func (o *TaskInstanceHistoryResponse) SetDagVersion(v DagVersionResponse)`

SetDagVersion sets DagVersion field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


