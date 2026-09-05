# DAGRunClearBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DryRun** | Pointer to **bool** |  | [optional] [default to true]
**OnlyFailed** | Pointer to **bool** |  | [optional] [default to false]
**OnlyNew** | Pointer to **bool** | Only queue newly added tasks in the latest DAG version without clearing existing tasks. | [optional] [default to false]
**RunOnLatestVersion** | Pointer to **bool** | (Experimental) Run on the latest bundle version of the Dag after clearing the Dag Run. | [optional] [default to false]

## Methods

### NewDAGRunClearBody

`func NewDAGRunClearBody() *DAGRunClearBody`

NewDAGRunClearBody instantiates a new DAGRunClearBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDAGRunClearBodyWithDefaults

`func NewDAGRunClearBodyWithDefaults() *DAGRunClearBody`

NewDAGRunClearBodyWithDefaults instantiates a new DAGRunClearBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDryRun

`func (o *DAGRunClearBody) GetDryRun() bool`

GetDryRun returns the DryRun field if non-nil, zero value otherwise.

### GetDryRunOk

`func (o *DAGRunClearBody) GetDryRunOk() (*bool, bool)`

GetDryRunOk returns a tuple with the DryRun field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDryRun

`func (o *DAGRunClearBody) SetDryRun(v bool)`

SetDryRun sets DryRun field to given value.

### HasDryRun

`func (o *DAGRunClearBody) HasDryRun() bool`

HasDryRun returns a boolean if a field has been set.

### GetOnlyFailed

`func (o *DAGRunClearBody) GetOnlyFailed() bool`

GetOnlyFailed returns the OnlyFailed field if non-nil, zero value otherwise.

### GetOnlyFailedOk

`func (o *DAGRunClearBody) GetOnlyFailedOk() (*bool, bool)`

GetOnlyFailedOk returns a tuple with the OnlyFailed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnlyFailed

`func (o *DAGRunClearBody) SetOnlyFailed(v bool)`

SetOnlyFailed sets OnlyFailed field to given value.

### HasOnlyFailed

`func (o *DAGRunClearBody) HasOnlyFailed() bool`

HasOnlyFailed returns a boolean if a field has been set.

### GetOnlyNew

`func (o *DAGRunClearBody) GetOnlyNew() bool`

GetOnlyNew returns the OnlyNew field if non-nil, zero value otherwise.

### GetOnlyNewOk

`func (o *DAGRunClearBody) GetOnlyNewOk() (*bool, bool)`

GetOnlyNewOk returns a tuple with the OnlyNew field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOnlyNew

`func (o *DAGRunClearBody) SetOnlyNew(v bool)`

SetOnlyNew sets OnlyNew field to given value.

### HasOnlyNew

`func (o *DAGRunClearBody) HasOnlyNew() bool`

HasOnlyNew returns a boolean if a field has been set.

### GetRunOnLatestVersion

`func (o *DAGRunClearBody) GetRunOnLatestVersion() bool`

GetRunOnLatestVersion returns the RunOnLatestVersion field if non-nil, zero value otherwise.

### GetRunOnLatestVersionOk

`func (o *DAGRunClearBody) GetRunOnLatestVersionOk() (*bool, bool)`

GetRunOnLatestVersionOk returns a tuple with the RunOnLatestVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunOnLatestVersion

`func (o *DAGRunClearBody) SetRunOnLatestVersion(v bool)`

SetRunOnLatestVersion sets RunOnLatestVersion field to given value.

### HasRunOnLatestVersion

`func (o *DAGRunClearBody) HasRunOnLatestVersion() bool`

HasRunOnLatestVersion returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


