# SchedulerInfoResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Status** | **string** |  | 
**LatestSchedulerHeartbeat** | **string** |  | 

## Methods

### NewSchedulerInfoResponse

`func NewSchedulerInfoResponse(status string, latestSchedulerHeartbeat string, ) *SchedulerInfoResponse`

NewSchedulerInfoResponse instantiates a new SchedulerInfoResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSchedulerInfoResponseWithDefaults

`func NewSchedulerInfoResponseWithDefaults() *SchedulerInfoResponse`

NewSchedulerInfoResponseWithDefaults instantiates a new SchedulerInfoResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStatus

`func (o *SchedulerInfoResponse) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SchedulerInfoResponse) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SchedulerInfoResponse) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetLatestSchedulerHeartbeat

`func (o *SchedulerInfoResponse) GetLatestSchedulerHeartbeat() string`

GetLatestSchedulerHeartbeat returns the LatestSchedulerHeartbeat field if non-nil, zero value otherwise.

### GetLatestSchedulerHeartbeatOk

`func (o *SchedulerInfoResponse) GetLatestSchedulerHeartbeatOk() (*string, bool)`

GetLatestSchedulerHeartbeatOk returns a tuple with the LatestSchedulerHeartbeat field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatestSchedulerHeartbeat

`func (o *SchedulerInfoResponse) SetLatestSchedulerHeartbeat(v string)`

SetLatestSchedulerHeartbeat sets LatestSchedulerHeartbeat field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


