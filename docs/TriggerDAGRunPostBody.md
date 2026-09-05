# TriggerDAGRunPostBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DagRunId** | Pointer to **string** |  | [optional] 
**DataIntervalStart** | Pointer to **time.Time** |  | [optional] 
**DataIntervalEnd** | Pointer to **time.Time** |  | [optional] 
**LogicalDate** | **time.Time** |  | 
**RunAfter** | Pointer to **time.Time** |  | [optional] 
**Conf** | Pointer to **map[string]interface{}** |  | [optional] 
**Note** | Pointer to **string** |  | [optional] 
**PartitionKey** | Pointer to **string** |  | [optional] 

## Methods

### NewTriggerDAGRunPostBody

`func NewTriggerDAGRunPostBody(logicalDate time.Time, ) *TriggerDAGRunPostBody`

NewTriggerDAGRunPostBody instantiates a new TriggerDAGRunPostBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTriggerDAGRunPostBodyWithDefaults

`func NewTriggerDAGRunPostBodyWithDefaults() *TriggerDAGRunPostBody`

NewTriggerDAGRunPostBodyWithDefaults instantiates a new TriggerDAGRunPostBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDagRunId

`func (o *TriggerDAGRunPostBody) GetDagRunId() string`

GetDagRunId returns the DagRunId field if non-nil, zero value otherwise.

### GetDagRunIdOk

`func (o *TriggerDAGRunPostBody) GetDagRunIdOk() (*string, bool)`

GetDagRunIdOk returns a tuple with the DagRunId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagRunId

`func (o *TriggerDAGRunPostBody) SetDagRunId(v string)`

SetDagRunId sets DagRunId field to given value.

### HasDagRunId

`func (o *TriggerDAGRunPostBody) HasDagRunId() bool`

HasDagRunId returns a boolean if a field has been set.

### GetDataIntervalStart

`func (o *TriggerDAGRunPostBody) GetDataIntervalStart() time.Time`

GetDataIntervalStart returns the DataIntervalStart field if non-nil, zero value otherwise.

### GetDataIntervalStartOk

`func (o *TriggerDAGRunPostBody) GetDataIntervalStartOk() (*time.Time, bool)`

GetDataIntervalStartOk returns a tuple with the DataIntervalStart field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataIntervalStart

`func (o *TriggerDAGRunPostBody) SetDataIntervalStart(v time.Time)`

SetDataIntervalStart sets DataIntervalStart field to given value.

### HasDataIntervalStart

`func (o *TriggerDAGRunPostBody) HasDataIntervalStart() bool`

HasDataIntervalStart returns a boolean if a field has been set.

### GetDataIntervalEnd

`func (o *TriggerDAGRunPostBody) GetDataIntervalEnd() time.Time`

GetDataIntervalEnd returns the DataIntervalEnd field if non-nil, zero value otherwise.

### GetDataIntervalEndOk

`func (o *TriggerDAGRunPostBody) GetDataIntervalEndOk() (*time.Time, bool)`

GetDataIntervalEndOk returns a tuple with the DataIntervalEnd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataIntervalEnd

`func (o *TriggerDAGRunPostBody) SetDataIntervalEnd(v time.Time)`

SetDataIntervalEnd sets DataIntervalEnd field to given value.

### HasDataIntervalEnd

`func (o *TriggerDAGRunPostBody) HasDataIntervalEnd() bool`

HasDataIntervalEnd returns a boolean if a field has been set.

### GetLogicalDate

`func (o *TriggerDAGRunPostBody) GetLogicalDate() time.Time`

GetLogicalDate returns the LogicalDate field if non-nil, zero value otherwise.

### GetLogicalDateOk

`func (o *TriggerDAGRunPostBody) GetLogicalDateOk() (*time.Time, bool)`

GetLogicalDateOk returns a tuple with the LogicalDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDate

`func (o *TriggerDAGRunPostBody) SetLogicalDate(v time.Time)`

SetLogicalDate sets LogicalDate field to given value.


### GetRunAfter

`func (o *TriggerDAGRunPostBody) GetRunAfter() time.Time`

GetRunAfter returns the RunAfter field if non-nil, zero value otherwise.

### GetRunAfterOk

`func (o *TriggerDAGRunPostBody) GetRunAfterOk() (*time.Time, bool)`

GetRunAfterOk returns a tuple with the RunAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfter

`func (o *TriggerDAGRunPostBody) SetRunAfter(v time.Time)`

SetRunAfter sets RunAfter field to given value.

### HasRunAfter

`func (o *TriggerDAGRunPostBody) HasRunAfter() bool`

HasRunAfter returns a boolean if a field has been set.

### GetConf

`func (o *TriggerDAGRunPostBody) GetConf() map[string]interface{}`

GetConf returns the Conf field if non-nil, zero value otherwise.

### GetConfOk

`func (o *TriggerDAGRunPostBody) GetConfOk() (*map[string]interface{}, bool)`

GetConfOk returns a tuple with the Conf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConf

`func (o *TriggerDAGRunPostBody) SetConf(v map[string]interface{})`

SetConf sets Conf field to given value.

### HasConf

`func (o *TriggerDAGRunPostBody) HasConf() bool`

HasConf returns a boolean if a field has been set.

### GetNote

`func (o *TriggerDAGRunPostBody) GetNote() string`

GetNote returns the Note field if non-nil, zero value otherwise.

### GetNoteOk

`func (o *TriggerDAGRunPostBody) GetNoteOk() (*string, bool)`

GetNoteOk returns a tuple with the Note field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNote

`func (o *TriggerDAGRunPostBody) SetNote(v string)`

SetNote sets Note field to given value.

### HasNote

`func (o *TriggerDAGRunPostBody) HasNote() bool`

HasNote returns a boolean if a field has been set.

### GetPartitionKey

`func (o *TriggerDAGRunPostBody) GetPartitionKey() string`

GetPartitionKey returns the PartitionKey field if non-nil, zero value otherwise.

### GetPartitionKeyOk

`func (o *TriggerDAGRunPostBody) GetPartitionKeyOk() (*string, bool)`

GetPartitionKeyOk returns a tuple with the PartitionKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartitionKey

`func (o *TriggerDAGRunPostBody) SetPartitionKey(v string)`

SetPartitionKey sets PartitionKey field to given value.

### HasPartitionKey

`func (o *TriggerDAGRunPostBody) HasPartitionKey() bool`

HasPartitionKey returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


