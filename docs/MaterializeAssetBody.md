# MaterializeAssetBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DagRunId** | Pointer to **string** |  | [optional] 
**DataIntervalStart** | Pointer to **time.Time** |  | [optional] 
**DataIntervalEnd** | Pointer to **time.Time** |  | [optional] 
**LogicalDate** | Pointer to **time.Time** |  | [optional] 
**RunAfter** | Pointer to **time.Time** |  | [optional] 
**Conf** | Pointer to **map[string]interface{}** |  | [optional] 
**Note** | Pointer to **string** |  | [optional] 
**PartitionKey** | Pointer to **string** |  | [optional] 

## Methods

### NewMaterializeAssetBody

`func NewMaterializeAssetBody() *MaterializeAssetBody`

NewMaterializeAssetBody instantiates a new MaterializeAssetBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMaterializeAssetBodyWithDefaults

`func NewMaterializeAssetBodyWithDefaults() *MaterializeAssetBody`

NewMaterializeAssetBodyWithDefaults instantiates a new MaterializeAssetBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDagRunId

`func (o *MaterializeAssetBody) GetDagRunId() string`

GetDagRunId returns the DagRunId field if non-nil, zero value otherwise.

### GetDagRunIdOk

`func (o *MaterializeAssetBody) GetDagRunIdOk() (*string, bool)`

GetDagRunIdOk returns a tuple with the DagRunId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagRunId

`func (o *MaterializeAssetBody) SetDagRunId(v string)`

SetDagRunId sets DagRunId field to given value.

### HasDagRunId

`func (o *MaterializeAssetBody) HasDagRunId() bool`

HasDagRunId returns a boolean if a field has been set.

### GetDataIntervalStart

`func (o *MaterializeAssetBody) GetDataIntervalStart() time.Time`

GetDataIntervalStart returns the DataIntervalStart field if non-nil, zero value otherwise.

### GetDataIntervalStartOk

`func (o *MaterializeAssetBody) GetDataIntervalStartOk() (*time.Time, bool)`

GetDataIntervalStartOk returns a tuple with the DataIntervalStart field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataIntervalStart

`func (o *MaterializeAssetBody) SetDataIntervalStart(v time.Time)`

SetDataIntervalStart sets DataIntervalStart field to given value.

### HasDataIntervalStart

`func (o *MaterializeAssetBody) HasDataIntervalStart() bool`

HasDataIntervalStart returns a boolean if a field has been set.

### GetDataIntervalEnd

`func (o *MaterializeAssetBody) GetDataIntervalEnd() time.Time`

GetDataIntervalEnd returns the DataIntervalEnd field if non-nil, zero value otherwise.

### GetDataIntervalEndOk

`func (o *MaterializeAssetBody) GetDataIntervalEndOk() (*time.Time, bool)`

GetDataIntervalEndOk returns a tuple with the DataIntervalEnd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataIntervalEnd

`func (o *MaterializeAssetBody) SetDataIntervalEnd(v time.Time)`

SetDataIntervalEnd sets DataIntervalEnd field to given value.

### HasDataIntervalEnd

`func (o *MaterializeAssetBody) HasDataIntervalEnd() bool`

HasDataIntervalEnd returns a boolean if a field has been set.

### GetLogicalDate

`func (o *MaterializeAssetBody) GetLogicalDate() time.Time`

GetLogicalDate returns the LogicalDate field if non-nil, zero value otherwise.

### GetLogicalDateOk

`func (o *MaterializeAssetBody) GetLogicalDateOk() (*time.Time, bool)`

GetLogicalDateOk returns a tuple with the LogicalDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDate

`func (o *MaterializeAssetBody) SetLogicalDate(v time.Time)`

SetLogicalDate sets LogicalDate field to given value.

### HasLogicalDate

`func (o *MaterializeAssetBody) HasLogicalDate() bool`

HasLogicalDate returns a boolean if a field has been set.

### GetRunAfter

`func (o *MaterializeAssetBody) GetRunAfter() time.Time`

GetRunAfter returns the RunAfter field if non-nil, zero value otherwise.

### GetRunAfterOk

`func (o *MaterializeAssetBody) GetRunAfterOk() (*time.Time, bool)`

GetRunAfterOk returns a tuple with the RunAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfter

`func (o *MaterializeAssetBody) SetRunAfter(v time.Time)`

SetRunAfter sets RunAfter field to given value.

### HasRunAfter

`func (o *MaterializeAssetBody) HasRunAfter() bool`

HasRunAfter returns a boolean if a field has been set.

### GetConf

`func (o *MaterializeAssetBody) GetConf() map[string]interface{}`

GetConf returns the Conf field if non-nil, zero value otherwise.

### GetConfOk

`func (o *MaterializeAssetBody) GetConfOk() (*map[string]interface{}, bool)`

GetConfOk returns a tuple with the Conf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConf

`func (o *MaterializeAssetBody) SetConf(v map[string]interface{})`

SetConf sets Conf field to given value.

### HasConf

`func (o *MaterializeAssetBody) HasConf() bool`

HasConf returns a boolean if a field has been set.

### GetNote

`func (o *MaterializeAssetBody) GetNote() string`

GetNote returns the Note field if non-nil, zero value otherwise.

### GetNoteOk

`func (o *MaterializeAssetBody) GetNoteOk() (*string, bool)`

GetNoteOk returns a tuple with the Note field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNote

`func (o *MaterializeAssetBody) SetNote(v string)`

SetNote sets Note field to given value.

### HasNote

`func (o *MaterializeAssetBody) HasNote() bool`

HasNote returns a boolean if a field has been set.

### GetPartitionKey

`func (o *MaterializeAssetBody) GetPartitionKey() string`

GetPartitionKey returns the PartitionKey field if non-nil, zero value otherwise.

### GetPartitionKeyOk

`func (o *MaterializeAssetBody) GetPartitionKeyOk() (*string, bool)`

GetPartitionKeyOk returns a tuple with the PartitionKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartitionKey

`func (o *MaterializeAssetBody) SetPartitionKey(v string)`

SetPartitionKey sets PartitionKey field to given value.

### HasPartitionKey

`func (o *MaterializeAssetBody) HasPartitionKey() bool`

HasPartitionKey returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


