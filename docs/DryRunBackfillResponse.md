# DryRunBackfillResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LogicalDate** | **NullableTime** |  | 
**PartitionKey** | **NullableString** |  | 
**PartitionDate** | **NullableTime** |  | 

## Methods

### NewDryRunBackfillResponse

`func NewDryRunBackfillResponse(logicalDate NullableTime, partitionKey NullableString, partitionDate NullableTime, ) *DryRunBackfillResponse`

NewDryRunBackfillResponse instantiates a new DryRunBackfillResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDryRunBackfillResponseWithDefaults

`func NewDryRunBackfillResponseWithDefaults() *DryRunBackfillResponse`

NewDryRunBackfillResponseWithDefaults instantiates a new DryRunBackfillResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLogicalDate

`func (o *DryRunBackfillResponse) GetLogicalDate() time.Time`

GetLogicalDate returns the LogicalDate field if non-nil, zero value otherwise.

### GetLogicalDateOk

`func (o *DryRunBackfillResponse) GetLogicalDateOk() (*time.Time, bool)`

GetLogicalDateOk returns a tuple with the LogicalDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogicalDate

`func (o *DryRunBackfillResponse) SetLogicalDate(v time.Time)`

SetLogicalDate sets LogicalDate field to given value.


### SetLogicalDateNil

`func (o *DryRunBackfillResponse) SetLogicalDateNil(b bool)`

 SetLogicalDateNil sets the value for LogicalDate to be an explicit nil

### UnsetLogicalDate
`func (o *DryRunBackfillResponse) UnsetLogicalDate()`

UnsetLogicalDate ensures that no value is present for LogicalDate, not even an explicit nil
### GetPartitionKey

`func (o *DryRunBackfillResponse) GetPartitionKey() string`

GetPartitionKey returns the PartitionKey field if non-nil, zero value otherwise.

### GetPartitionKeyOk

`func (o *DryRunBackfillResponse) GetPartitionKeyOk() (*string, bool)`

GetPartitionKeyOk returns a tuple with the PartitionKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartitionKey

`func (o *DryRunBackfillResponse) SetPartitionKey(v string)`

SetPartitionKey sets PartitionKey field to given value.


### SetPartitionKeyNil

`func (o *DryRunBackfillResponse) SetPartitionKeyNil(b bool)`

 SetPartitionKeyNil sets the value for PartitionKey to be an explicit nil

### UnsetPartitionKey
`func (o *DryRunBackfillResponse) UnsetPartitionKey()`

UnsetPartitionKey ensures that no value is present for PartitionKey, not even an explicit nil
### GetPartitionDate

`func (o *DryRunBackfillResponse) GetPartitionDate() time.Time`

GetPartitionDate returns the PartitionDate field if non-nil, zero value otherwise.

### GetPartitionDateOk

`func (o *DryRunBackfillResponse) GetPartitionDateOk() (*time.Time, bool)`

GetPartitionDateOk returns a tuple with the PartitionDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartitionDate

`func (o *DryRunBackfillResponse) SetPartitionDate(v time.Time)`

SetPartitionDate sets PartitionDate field to given value.


### SetPartitionDateNil

`func (o *DryRunBackfillResponse) SetPartitionDateNil(b bool)`

 SetPartitionDateNil sets the value for PartitionDate to be an explicit nil

### UnsetPartitionDate
`func (o *DryRunBackfillResponse) UnsetPartitionDate()`

UnsetPartitionDate ensures that no value is present for PartitionDate, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


