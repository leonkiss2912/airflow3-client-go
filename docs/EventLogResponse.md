# EventLogResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EventLogId** | **int32** |  | 
**When** | **time.Time** |  | 
**DagId** | **string** |  | 
**TaskId** | **string** |  | 
**RunId** | **string** |  | 
**MapIndex** | **int32** |  | 
**TryNumber** | **int32** |  | 
**Event** | **string** |  | 
**LogicalDate** | **time.Time** |  | 
**Owner** | **string** |  | 
**Extra** | **string** |  | 
**DagDisplayName** | Pointer to **string** |  | [optional] 
**TaskDisplayName** | Pointer to **string** |  | [optional] 

## Methods

### NewEventLogResponse

`func NewEventLogResponse(eventLogId int32, when time.Time, dagId string, taskId string, runId string, mapIndex int32, tryNumber int32, event string, logicalDate time.Time, owner string, extra string, ) *EventLogResponse`

NewEventLogResponse instantiates a new EventLogResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEventLogResponseWithDefaults

`func NewEventLogResponseWithDefaults() *EventLogResponse`

NewEventLogResponseWithDefaults instantiates a new EventLogResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEventLogId

`func (o *EventLogResponse) GetEventLogId() int32`

GetEventLogId returns the EventLogId field if non-nil, zero value otherwise.

### GetEventLogIdOk

`func (o *EventLogResponse) GetEventLogIdOk() (*int32, bool)`

GetEventLogIdOk returns a tuple with the EventLogId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventLogId

`func (o *EventLogResponse) SetEventLogId(v int32)`

SetEventLogId sets EventLogId field to given value.


### GetWhen

`func (o *EventLogResponse) GetWhen() time.Time`

GetWhen returns the When field if non-nil, zero value otherwise.

### GetWhenOk

`func (o *EventLogResponse) GetWhenOk() (*time.Time, bool)`

GetWhenOk returns a tuple with the When field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWhen

`func (o *EventLogResponse) SetWhen(v time.Time)`

SetWhen sets When field to given value.


### GetDagId

`func (o *EventLogResponse) GetDagId() string`

GetDagId returns the DagId field if non-nil, zero value otherwise.

### GetDagIdOk

`func (o *EventLogResponse) GetDagIdOk() (*string, bool)`

GetDagIdOk returns a tuple with the DagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagId

`func (o *EventLogResponse) SetDagId(v string)`

SetDagId sets DagId field to given value.


### GetTaskId

`func (o *EventLogResponse) GetTaskId() string`

GetTaskId returns the TaskId field if non-nil, zero value otherwise.

### GetTaskIdOk

`func (o *EventLogResponse) GetTaskIdOk() (*string, bool)`

GetTaskIdOk returns a tuple with the TaskId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskId

`func (o *EventLogResponse) SetTaskId(v string)`

SetTaskId sets TaskId field to given value.


### GetRunId

`func (o *EventLogResponse) GetRunId() string`

GetRunId returns the RunId field if non-nil, zero value otherwise.

### GetRunIdOk

`func (o *EventLogResponse) GetRunIdOk() (*string, bool)`

GetRunIdOk returns a tuple with the RunId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunId

`func (o *EventLogResponse) SetRunId(v string)`

SetRunId sets RunId field to given value.


### GetMapIndex

`func (o *EventLogResponse) GetMapIndex() int32`

GetMapIndex returns the MapIndex field if non-nil, zero value otherwise.

### GetMapIndexOk

`func (o *EventLogResponse) GetMapIndexOk() (*int32, bool)`

GetMapIndexOk returns a tuple with the MapIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMapIndex

`func (o *EventLogResponse) SetMapIndex(v int32)`

SetMapIndex sets MapIndex field to given value.


### GetTryNumber

`func (o *EventLogResponse) GetTryNumber() int32`

GetTryNumber returns the TryNumber field if non-nil, zero value otherwise.

### GetTryNumberOk

`func (o *EventLogResponse) GetTryNumberOk() (*int32, bool)`

GetTryNumberOk returns a tuple with the TryNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTryNumber

`func (o *EventLogResponse) SetTryNumber(v int32)`

SetTryNumber sets TryNumber field to given value.


### GetEvent

`func (o *EventLogResponse) GetEvent() string`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *EventLogResponse) GetEventOk() (*string, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *EventLogResponse) SetEvent(v string)`

SetEvent sets Event field to given value.


### GetLogicalDate

`func (o *EventLogResponse) GetLogicalDate() time.Time`

GetLogicalDate returns the LogicalDate field if non-nil, zero value otherwise.

### GetLogicalDateOk

`func (o *EventLogResponse) GetLogicalDateOk() (*time.Time, bool)`

GetLogicalDateOk returns a tuple with the LogicalDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDate

`func (o *EventLogResponse) SetLogicalDate(v time.Time)`

SetLogicalDate sets LogicalDate field to given value.


### GetOwner

`func (o *EventLogResponse) GetOwner() string`

GetOwner returns the Owner field if non-nil, zero value otherwise.

### GetOwnerOk

`func (o *EventLogResponse) GetOwnerOk() (*string, bool)`

GetOwnerOk returns a tuple with the Owner field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwner

`func (o *EventLogResponse) SetOwner(v string)`

SetOwner sets Owner field to given value.


### GetExtra

`func (o *EventLogResponse) GetExtra() string`

GetExtra returns the Extra field if non-nil, zero value otherwise.

### GetExtraOk

`func (o *EventLogResponse) GetExtraOk() (*string, bool)`

GetExtraOk returns a tuple with the Extra field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtra

`func (o *EventLogResponse) SetExtra(v string)`

SetExtra sets Extra field to given value.


### GetDagDisplayName

`func (o *EventLogResponse) GetDagDisplayName() string`

GetDagDisplayName returns the DagDisplayName field if non-nil, zero value otherwise.

### GetDagDisplayNameOk

`func (o *EventLogResponse) GetDagDisplayNameOk() (*string, bool)`

GetDagDisplayNameOk returns a tuple with the DagDisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagDisplayName

`func (o *EventLogResponse) SetDagDisplayName(v string)`

SetDagDisplayName sets DagDisplayName field to given value.

### HasDagDisplayName

`func (o *EventLogResponse) HasDagDisplayName() bool`

HasDagDisplayName returns a boolean if a field has been set.

### GetTaskDisplayName

`func (o *EventLogResponse) GetTaskDisplayName() string`

GetTaskDisplayName returns the TaskDisplayName field if non-nil, zero value otherwise.

### GetTaskDisplayNameOk

`func (o *EventLogResponse) GetTaskDisplayNameOk() (*string, bool)`

GetTaskDisplayNameOk returns a tuple with the TaskDisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskDisplayName

`func (o *EventLogResponse) SetTaskDisplayName(v string)`

SetTaskDisplayName sets TaskDisplayName field to given value.

### HasTaskDisplayName

`func (o *EventLogResponse) HasTaskDisplayName() bool`

HasTaskDisplayName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


