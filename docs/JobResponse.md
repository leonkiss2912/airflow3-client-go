# JobResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int32** |  | 
**DagId** | **string** |  | 
**State** | **string** |  | 
**JobType** | **string** |  | 
**StartDate** | **time.Time** |  | 
**EndDate** | **time.Time** |  | 
**LatestHeartbeat** | **time.Time** |  | 
**ExecutorClass** | **string** |  | 
**Hostname** | **string** |  | 
**Unixname** | **string** |  | 
**DagDisplayName** | Pointer to **string** |  | [optional] 

## Methods

### NewJobResponse

`func NewJobResponse(id int32, dagId string, state string, jobType string, startDate time.Time, endDate time.Time, latestHeartbeat time.Time, executorClass string, hostname string, unixname string, ) *JobResponse`

NewJobResponse instantiates a new JobResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewJobResponseWithDefaults

`func NewJobResponseWithDefaults() *JobResponse`

NewJobResponseWithDefaults instantiates a new JobResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *JobResponse) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *JobResponse) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *JobResponse) SetId(v int32)`

SetId sets Id field to given value.


### GetDagId

`func (o *JobResponse) GetDagId() string`

GetDagId returns the DagId field if non-nil, zero value otherwise.

### GetDagIdOk

`func (o *JobResponse) GetDagIdOk() (*string, bool)`

GetDagIdOk returns a tuple with the DagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagId

`func (o *JobResponse) SetDagId(v string)`

SetDagId sets DagId field to given value.


### GetState

`func (o *JobResponse) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *JobResponse) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *JobResponse) SetState(v string)`

SetState sets State field to given value.


### GetJobType

`func (o *JobResponse) GetJobType() string`

GetJobType returns the JobType field if non-nil, zero value otherwise.

### GetJobTypeOk

`func (o *JobResponse) GetJobTypeOk() (*string, bool)`

GetJobTypeOk returns a tuple with the JobType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJobType

`func (o *JobResponse) SetJobType(v string)`

SetJobType sets JobType field to given value.


### GetStartDate

`func (o *JobResponse) GetStartDate() time.Time`

GetStartDate returns the StartDate field if non-nil, zero value otherwise.

### GetStartDateOk

`func (o *JobResponse) GetStartDateOk() (*time.Time, bool)`

GetStartDateOk returns a tuple with the StartDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartDate

`func (o *JobResponse) SetStartDate(v time.Time)`

SetStartDate sets StartDate field to given value.


### GetEndDate

`func (o *JobResponse) GetEndDate() time.Time`

GetEndDate returns the EndDate field if non-nil, zero value otherwise.

### GetEndDateOk

`func (o *JobResponse) GetEndDateOk() (*time.Time, bool)`

GetEndDateOk returns a tuple with the EndDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndDate

`func (o *JobResponse) SetEndDate(v time.Time)`

SetEndDate sets EndDate field to given value.


### GetLatestHeartbeat

`func (o *JobResponse) GetLatestHeartbeat() time.Time`

GetLatestHeartbeat returns the LatestHeartbeat field if non-nil, zero value otherwise.

### GetLatestHeartbeatOk

`func (o *JobResponse) GetLatestHeartbeatOk() (*time.Time, bool)`

GetLatestHeartbeatOk returns a tuple with the LatestHeartbeat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatestHeartbeat

`func (o *JobResponse) SetLatestHeartbeat(v time.Time)`

SetLatestHeartbeat sets LatestHeartbeat field to given value.


### GetExecutorClass

`func (o *JobResponse) GetExecutorClass() string`

GetExecutorClass returns the ExecutorClass field if non-nil, zero value otherwise.

### GetExecutorClassOk

`func (o *JobResponse) GetExecutorClassOk() (*string, bool)`

GetExecutorClassOk returns a tuple with the ExecutorClass field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutorClass

`func (o *JobResponse) SetExecutorClass(v string)`

SetExecutorClass sets ExecutorClass field to given value.


### GetHostname

`func (o *JobResponse) GetHostname() string`

GetHostname returns the Hostname field if non-nil, zero value otherwise.

### GetHostnameOk

`func (o *JobResponse) GetHostnameOk() (*string, bool)`

GetHostnameOk returns a tuple with the Hostname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHostname

`func (o *JobResponse) SetHostname(v string)`

SetHostname sets Hostname field to given value.


### GetUnixname

`func (o *JobResponse) GetUnixname() string`

GetUnixname returns the Unixname field if non-nil, zero value otherwise.

### GetUnixnameOk

`func (o *JobResponse) GetUnixnameOk() (*string, bool)`

GetUnixnameOk returns a tuple with the Unixname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnixname

`func (o *JobResponse) SetUnixname(v string)`

SetUnixname sets Unixname field to given value.


### GetDagDisplayName

`func (o *JobResponse) GetDagDisplayName() string`

GetDagDisplayName returns the DagDisplayName field if non-nil, zero value otherwise.

### GetDagDisplayNameOk

`func (o *JobResponse) GetDagDisplayNameOk() (*string, bool)`

GetDagDisplayNameOk returns a tuple with the DagDisplayName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDagDisplayName

`func (o *JobResponse) SetDagDisplayName(v string)`

SetDagDisplayName sets DagDisplayName field to given value.

### HasDagDisplayName

`func (o *JobResponse) HasDagDisplayName() bool`

HasDagDisplayName returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


