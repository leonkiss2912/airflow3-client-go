# DAGRunCollectionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DagRuns** | [**[]DAGRunResponse**](DAGRunResponse.md) |  | 
**TotalEntries** | Pointer to **NullableInt32** | Total number of matching items. Populated for offset pagination, &#x60;&#x60;null&#x60;&#x60; when using cursor pagination. | [optional] 
**NextCursor** | Pointer to **NullableString** | Token pointing to the next page. Populated for cursor pagination, &#x60;&#x60;null&#x60;&#x60; when using offset pagination or when there is no next page. | [optional] 
**PreviousCursor** | Pointer to **NullableString** | Token pointing to the previous page. Populated for cursor pagination, &#x60;&#x60;null&#x60;&#x60; when using offset pagination or when on the first page. | [optional] 

## Methods

### NewDAGRunCollectionResponse

`func NewDAGRunCollectionResponse(dagRuns []DAGRunResponse, ) *DAGRunCollectionResponse`

NewDAGRunCollectionResponse instantiates a new DAGRunCollectionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDAGRunCollectionResponseWithDefaults

`func NewDAGRunCollectionResponseWithDefaults() *DAGRunCollectionResponse`

NewDAGRunCollectionResponseWithDefaults instantiates a new DAGRunCollectionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDagRuns

`func (o *DAGRunCollectionResponse) GetDagRuns() []DAGRunResponse`

GetDagRuns returns the DagRuns field if non-nil, zero value otherwise.

### GetDagRunsOk

`func (o *DAGRunCollectionResponse) GetDagRunsOk() (*[]DAGRunResponse, bool)`

GetDagRunsOk returns a tuple with the DagRuns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagRuns

`func (o *DAGRunCollectionResponse) SetDagRuns(v []DAGRunResponse)`

SetDagRuns sets DagRuns field to given value.


### GetTotalEntries

`func (o *DAGRunCollectionResponse) GetTotalEntries() int32`

GetTotalEntries returns the TotalEntries field if non-nil, zero value otherwise.

### GetTotalEntriesOk

`func (o *DAGRunCollectionResponse) GetTotalEntriesOk() (*int32, bool)`

GetTotalEntriesOk returns a tuple with the TotalEntries field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalEntries

`func (o *DAGRunCollectionResponse) SetTotalEntries(v int32)`

SetTotalEntries sets TotalEntries field to given value.

### HasTotalEntries

`func (o *DAGRunCollectionResponse) HasTotalEntries() bool`

HasTotalEntries returns a boolean if a field has been set.

### SetTotalEntriesNil

`func (o *DAGRunCollectionResponse) SetTotalEntriesNil(b bool)`

 SetTotalEntriesNil sets the value for TotalEntries to be an explicit nil

### UnsetTotalEntries
`func (o *DAGRunCollectionResponse) UnsetTotalEntries()`

UnsetTotalEntries ensures that no value is present for TotalEntries, not even an explicit nil
### GetNextCursor

`func (o *DAGRunCollectionResponse) GetNextCursor() string`

GetNextCursor returns the NextCursor field if non-nil, zero value otherwise.

### GetNextCursorOk

`func (o *DAGRunCollectionResponse) GetNextCursorOk() (*string, bool)`

GetNextCursorOk returns a tuple with the NextCursor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextCursor

`func (o *DAGRunCollectionResponse) SetNextCursor(v string)`

SetNextCursor sets NextCursor field to given value.

### HasNextCursor

`func (o *DAGRunCollectionResponse) HasNextCursor() bool`

HasNextCursor returns a boolean if a field has been set.

### SetNextCursorNil

`func (o *DAGRunCollectionResponse) SetNextCursorNil(b bool)`

 SetNextCursorNil sets the value for NextCursor to be an explicit nil

### UnsetNextCursor
`func (o *DAGRunCollectionResponse) UnsetNextCursor()`

UnsetNextCursor ensures that no value is present for NextCursor, not even an explicit nil
### GetPreviousCursor

`func (o *DAGRunCollectionResponse) GetPreviousCursor() string`

GetPreviousCursor returns the PreviousCursor field if non-nil, zero value otherwise.

### GetPreviousCursorOk

`func (o *DAGRunCollectionResponse) GetPreviousCursorOk() (*string, bool)`

GetPreviousCursorOk returns a tuple with the PreviousCursor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreviousCursor

`func (o *DAGRunCollectionResponse) SetPreviousCursor(v string)`

SetPreviousCursor sets PreviousCursor field to given value.

### HasPreviousCursor

`func (o *DAGRunCollectionResponse) HasPreviousCursor() bool`

HasPreviousCursor returns a boolean if a field has been set.

### SetPreviousCursorNil

`func (o *DAGRunCollectionResponse) SetPreviousCursorNil(b bool)`

 SetPreviousCursorNil sets the value for PreviousCursor to be an explicit nil

### UnsetPreviousCursor
`func (o *DAGRunCollectionResponse) UnsetPreviousCursor()`

UnsetPreviousCursor ensures that no value is present for PreviousCursor, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


