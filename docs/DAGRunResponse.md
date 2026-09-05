# DAGRunResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DagRunId** | **string** |  | 
**DagId** | **string** |  | 
**LogicalDate** | **time.Time** |  | 
**QueuedAt** | **time.Time** |  | 
**StartDate** | **time.Time** |  | 
**EndDate** | **time.Time** |  | 
**Duration** | **float32** |  | 
**DataIntervalStart** | **time.Time** |  | 
**DataIntervalEnd** | **time.Time** |  | 
**RunAfter** | **time.Time** |  | 
**LastSchedulingDecision** | **time.Time** |  | 
**RunType** | [**DagRunType**](DagRunType.md) |  | 
**State** | [**DagRunState**](DagRunState.md) |  | 
**TriggeredBy** | [**DagRunTriggeredByType**](DagRunTriggeredByType.md) |  | 
**TriggeringUserName** | **string** |  | 
**Conf** | **map[string]interface{}** |  | 
**Note** | **string** |  | 
**DagVersions** | [**[]DagVersionResponse**](DagVersionResponse.md) |  | 
**BundleVersion** | **string** |  | 
**DagDisplayName** | **string** |  | 
**PartitionKey** | **string** |  | 

## Methods

### NewDAGRunResponse

`func NewDAGRunResponse(dagRunId string, dagId string, logicalDate time.Time, queuedAt time.Time, startDate time.Time, endDate time.Time, duration float32, dataIntervalStart time.Time, dataIntervalEnd time.Time, runAfter time.Time, lastSchedulingDecision time.Time, runType DagRunType, state DagRunState, triggeredBy DagRunTriggeredByType, triggeringUserName string, conf map[string]interface{}, note string, dagVersions []DagVersionResponse, bundleVersion string, dagDisplayName string, partitionKey string, ) *DAGRunResponse`

NewDAGRunResponse instantiates a new DAGRunResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDAGRunResponseWithDefaults

`func NewDAGRunResponseWithDefaults() *DAGRunResponse`

NewDAGRunResponseWithDefaults instantiates a new DAGRunResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDagRunId

`func (o *DAGRunResponse) GetDagRunId() string`

GetDagRunId returns the DagRunId field if non-nil, zero value otherwise.

### GetDagRunIdOk

`func (o *DAGRunResponse) GetDagRunIdOk() (*string, bool)`

GetDagRunIdOk returns a tuple with the DagRunId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagRunId

`func (o *DAGRunResponse) SetDagRunId(v string)`

SetDagRunId sets DagRunId field to given value.


### GetDagId

`func (o *DAGRunResponse) GetDagId() string`

GetDagId returns the DagId field if non-nil, zero value otherwise.

### GetDagIdOk

`func (o *DAGRunResponse) GetDagIdOk() (*string, bool)`

GetDagIdOk returns a tuple with the DagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagId

`func (o *DAGRunResponse) SetDagId(v string)`

SetDagId sets DagId field to given value.


### GetLogicalDate

`func (o *DAGRunResponse) GetLogicalDate() time.Time`

GetLogicalDate returns the LogicalDate field if non-nil, zero value otherwise.

### GetLogicalDateOk

`func (o *DAGRunResponse) GetLogicalDateOk() (*time.Time, bool)`

GetLogicalDateOk returns a tuple with the LogicalDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDate

`func (o *DAGRunResponse) SetLogicalDate(v time.Time)`

SetLogicalDate sets LogicalDate field to given value.


### GetQueuedAt

`func (o *DAGRunResponse) GetQueuedAt() time.Time`

GetQueuedAt returns the QueuedAt field if non-nil, zero value otherwise.

### GetQueuedAtOk

`func (o *DAGRunResponse) GetQueuedAtOk() (*time.Time, bool)`

GetQueuedAtOk returns a tuple with the QueuedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQueuedAt

`func (o *DAGRunResponse) SetQueuedAt(v time.Time)`

SetQueuedAt sets QueuedAt field to given value.


### GetStartDate

`func (o *DAGRunResponse) GetStartDate() time.Time`

GetStartDate returns the StartDate field if non-nil, zero value otherwise.

### GetStartDateOk

`func (o *DAGRunResponse) GetStartDateOk() (*time.Time, bool)`

GetStartDateOk returns a tuple with the StartDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDate

`func (o *DAGRunResponse) SetStartDate(v time.Time)`

SetStartDate sets StartDate field to given value.


### GetEndDate

`func (o *DAGRunResponse) GetEndDate() time.Time`

GetEndDate returns the EndDate field if non-nil, zero value otherwise.

### GetEndDateOk

`func (o *DAGRunResponse) GetEndDateOk() (*time.Time, bool)`

GetEndDateOk returns a tuple with the EndDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDate

`func (o *DAGRunResponse) SetEndDate(v time.Time)`

SetEndDate sets EndDate field to given value.


### GetDuration

`func (o *DAGRunResponse) GetDuration() float32`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *DAGRunResponse) GetDurationOk() (*float32, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *DAGRunResponse) SetDuration(v float32)`

SetDuration sets Duration field to given value.


### GetDataIntervalStart

`func (o *DAGRunResponse) GetDataIntervalStart() time.Time`

GetDataIntervalStart returns the DataIntervalStart field if non-nil, zero value otherwise.

### GetDataIntervalStartOk

`func (o *DAGRunResponse) GetDataIntervalStartOk() (*time.Time, bool)`

GetDataIntervalStartOk returns a tuple with the DataIntervalStart field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataIntervalStart

`func (o *DAGRunResponse) SetDataIntervalStart(v time.Time)`

SetDataIntervalStart sets DataIntervalStart field to given value.


### GetDataIntervalEnd

`func (o *DAGRunResponse) GetDataIntervalEnd() time.Time`

GetDataIntervalEnd returns the DataIntervalEnd field if non-nil, zero value otherwise.

### GetDataIntervalEndOk

`func (o *DAGRunResponse) GetDataIntervalEndOk() (*time.Time, bool)`

GetDataIntervalEndOk returns a tuple with the DataIntervalEnd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataIntervalEnd

`func (o *DAGRunResponse) SetDataIntervalEnd(v time.Time)`

SetDataIntervalEnd sets DataIntervalEnd field to given value.


### GetRunAfter

`func (o *DAGRunResponse) GetRunAfter() time.Time`

GetRunAfter returns the RunAfter field if non-nil, zero value otherwise.

### GetRunAfterOk

`func (o *DAGRunResponse) GetRunAfterOk() (*time.Time, bool)`

GetRunAfterOk returns a tuple with the RunAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunAfter

`func (o *DAGRunResponse) SetRunAfter(v time.Time)`

SetRunAfter sets RunAfter field to given value.


### GetLastSchedulingDecision

`func (o *DAGRunResponse) GetLastSchedulingDecision() time.Time`

GetLastSchedulingDecision returns the LastSchedulingDecision field if non-nil, zero value otherwise.

### GetLastSchedulingDecisionOk

`func (o *DAGRunResponse) GetLastSchedulingDecisionOk() (*time.Time, bool)`

GetLastSchedulingDecisionOk returns a tuple with the LastSchedulingDecision field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSchedulingDecision

`func (o *DAGRunResponse) SetLastSchedulingDecision(v time.Time)`

SetLastSchedulingDecision sets LastSchedulingDecision field to given value.


### GetRunType

`func (o *DAGRunResponse) GetRunType() DagRunType`

GetRunType returns the RunType field if non-nil, zero value otherwise.

### GetRunTypeOk

`func (o *DAGRunResponse) GetRunTypeOk() (*DagRunType, bool)`

GetRunTypeOk returns a tuple with the RunType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRunType

`func (o *DAGRunResponse) SetRunType(v DagRunType)`

SetRunType sets RunType field to given value.


### GetState

`func (o *DAGRunResponse) GetState() DagRunState`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *DAGRunResponse) GetStateOk() (*DagRunState, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *DAGRunResponse) SetState(v DagRunState)`

SetState sets State field to given value.


### GetTriggeredBy

`func (o *DAGRunResponse) GetTriggeredBy() DagRunTriggeredByType`

GetTriggeredBy returns the TriggeredBy field if non-nil, zero value otherwise.

### GetTriggeredByOk

`func (o *DAGRunResponse) GetTriggeredByOk() (*DagRunTriggeredByType, bool)`

GetTriggeredByOk returns a tuple with the TriggeredBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTriggeredBy

`func (o *DAGRunResponse) SetTriggeredBy(v DagRunTriggeredByType)`

SetTriggeredBy sets TriggeredBy field to given value.


### GetTriggeringUserName

`func (o *DAGRunResponse) GetTriggeringUserName() string`

GetTriggeringUserName returns the TriggeringUserName field if non-nil, zero value otherwise.

### GetTriggeringUserNameOk

`func (o *DAGRunResponse) GetTriggeringUserNameOk() (*string, bool)`

GetTriggeringUserNameOk returns a tuple with the TriggeringUserName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTriggeringUserName

`func (o *DAGRunResponse) SetTriggeringUserName(v string)`

SetTriggeringUserName sets TriggeringUserName field to given value.


### GetConf

`func (o *DAGRunResponse) GetConf() map[string]interface{}`

GetConf returns the Conf field if non-nil, zero value otherwise.

### GetConfOk

`func (o *DAGRunResponse) GetConfOk() (*map[string]interface{}, bool)`

GetConfOk returns a tuple with the Conf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConf

`func (o *DAGRunResponse) SetConf(v map[string]interface{})`

SetConf sets Conf field to given value.


### GetNote

`func (o *DAGRunResponse) GetNote() string`

GetNote returns the Note field if non-nil, zero value otherwise.

### GetNoteOk

`func (o *DAGRunResponse) GetNoteOk() (*string, bool)`

GetNoteOk returns a tuple with the Note field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNote

`func (o *DAGRunResponse) SetNote(v string)`

SetNote sets Note field to given value.


### GetDagVersions

`func (o *DAGRunResponse) GetDagVersions() []DagVersionResponse`

GetDagVersions returns the DagVersions field if non-nil, zero value otherwise.

### GetDagVersionsOk

`func (o *DAGRunResponse) GetDagVersionsOk() (*[]DagVersionResponse, bool)`

GetDagVersionsOk returns a tuple with the DagVersions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagVersions

`func (o *DAGRunResponse) SetDagVersions(v []DagVersionResponse)`

SetDagVersions sets DagVersions field to given value.


### GetBundleVersion

`func (o *DAGRunResponse) GetBundleVersion() string`

GetBundleVersion returns the BundleVersion field if non-nil, zero value otherwise.

### GetBundleVersionOk

`func (o *DAGRunResponse) GetBundleVersionOk() (*string, bool)`

GetBundleVersionOk returns a tuple with the BundleVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBundleVersion

`func (o *DAGRunResponse) SetBundleVersion(v string)`

SetBundleVersion sets BundleVersion field to given value.


### GetDagDisplayName

`func (o *DAGRunResponse) GetDagDisplayName() string`

GetDagDisplayName returns the DagDisplayName field if non-nil, zero value otherwise.

### GetDagDisplayNameOk

`func (o *DAGRunResponse) GetDagDisplayNameOk() (*string, bool)`

GetDagDisplayNameOk returns a tuple with the DagDisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagDisplayName

`func (o *DAGRunResponse) SetDagDisplayName(v string)`

SetDagDisplayName sets DagDisplayName field to given value.


### GetPartitionKey

`func (o *DAGRunResponse) GetPartitionKey() string`

GetPartitionKey returns the PartitionKey field if non-nil, zero value otherwise.

### GetPartitionKeyOk

`func (o *DAGRunResponse) GetPartitionKeyOk() (*string, bool)`

GetPartitionKeyOk returns a tuple with the PartitionKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartitionKey

`func (o *DAGRunResponse) SetPartitionKey(v string)`

SetPartitionKey sets PartitionKey field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


