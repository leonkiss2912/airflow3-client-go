# TaskInstanceCollectionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TaskInstances** | [**[]TaskInstanceResponse**](TaskInstanceResponse.md) |  | 
**TotalEntries** | Pointer to **int32** | Total number of matching items. Populated for offset pagination, &#x60;&#x60;null&#x60;&#x60; when using cursor pagination. | [optional] 
**NextCursor** | Pointer to **string** | Token pointing to the next page. Populated for cursor pagination, &#x60;&#x60;null&#x60;&#x60; when using offset pagination or when there is no next page. | [optional] 
**PreviousCursor** | Pointer to **string** | Token pointing to the previous page. Populated for cursor pagination, &#x60;&#x60;null&#x60;&#x60; when using offset pagination or when on the first page. | [optional] 

## Methods

### NewTaskInstanceCollectionResponse

`func NewTaskInstanceCollectionResponse(taskInstances []TaskInstanceResponse, ) *TaskInstanceCollectionResponse`

NewTaskInstanceCollectionResponse instantiates a new TaskInstanceCollectionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTaskInstanceCollectionResponseWithDefaults

`func NewTaskInstanceCollectionResponseWithDefaults() *TaskInstanceCollectionResponse`

NewTaskInstanceCollectionResponseWithDefaults instantiates a new TaskInstanceCollectionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTaskInstances

`func (o *TaskInstanceCollectionResponse) GetTaskInstances() []TaskInstanceResponse`

GetTaskInstances returns the TaskInstances field if non-nil, zero value otherwise.

### GetTaskInstancesOk

`func (o *TaskInstanceCollectionResponse) GetTaskInstancesOk() (*[]TaskInstanceResponse, bool)`

GetTaskInstancesOk returns a tuple with the TaskInstances field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskInstances

`func (o *TaskInstanceCollectionResponse) SetTaskInstances(v []TaskInstanceResponse)`

SetTaskInstances sets TaskInstances field to given value.


### GetTotalEntries

`func (o *TaskInstanceCollectionResponse) GetTotalEntries() int32`

GetTotalEntries returns the TotalEntries field if non-nil, zero value otherwise.

### GetTotalEntriesOk

`func (o *TaskInstanceCollectionResponse) GetTotalEntriesOk() (*int32, bool)`

GetTotalEntriesOk returns a tuple with the TotalEntries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalEntries

`func (o *TaskInstanceCollectionResponse) SetTotalEntries(v int32)`

SetTotalEntries sets TotalEntries field to given value.

### HasTotalEntries

`func (o *TaskInstanceCollectionResponse) HasTotalEntries() bool`

HasTotalEntries returns a boolean if a field has been set.

### GetNextCursor

`func (o *TaskInstanceCollectionResponse) GetNextCursor() string`

GetNextCursor returns the NextCursor field if non-nil, zero value otherwise.

### GetNextCursorOk

`func (o *TaskInstanceCollectionResponse) GetNextCursorOk() (*string, bool)`

GetNextCursorOk returns a tuple with the NextCursor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextCursor

`func (o *TaskInstanceCollectionResponse) SetNextCursor(v string)`

SetNextCursor sets NextCursor field to given value.

### HasNextCursor

`func (o *TaskInstanceCollectionResponse) HasNextCursor() bool`

HasNextCursor returns a boolean if a field has been set.

### GetPreviousCursor

`func (o *TaskInstanceCollectionResponse) GetPreviousCursor() string`

GetPreviousCursor returns the PreviousCursor field if non-nil, zero value otherwise.

### GetPreviousCursorOk

`func (o *TaskInstanceCollectionResponse) GetPreviousCursorOk() (*string, bool)`

GetPreviousCursorOk returns a tuple with the PreviousCursor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreviousCursor

`func (o *TaskInstanceCollectionResponse) SetPreviousCursor(v string)`

SetPreviousCursor sets PreviousCursor field to given value.

### HasPreviousCursor

`func (o *TaskInstanceCollectionResponse) HasPreviousCursor() bool`

HasPreviousCursor returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


