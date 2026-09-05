# AssetEventResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **int32** |  | 
**AssetId** | **int32** |  | 
**Uri** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**Group** | Pointer to **string** |  | [optional] 
**Extra** | Pointer to **map[string]interface{}** |  | [optional] 
**SourceTaskId** | Pointer to **string** |  | [optional] 
**SourceDagId** | Pointer to **string** |  | [optional] 
**SourceRunId** | Pointer to **string** |  | [optional] 
**SourceMapIndex** | **int32** |  | 
**CreatedDagruns** | [**[]DagRunAssetReference**](DagRunAssetReference.md) |  | 
**Timestamp** | **time.Time** |  | 
**PartitionKey** | Pointer to **string** |  | [optional] 

## Methods

### NewAssetEventResponse

`func NewAssetEventResponse(id int32, assetId int32, sourceMapIndex int32, createdDagruns []DagRunAssetReference, timestamp time.Time, ) *AssetEventResponse`

NewAssetEventResponse instantiates a new AssetEventResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAssetEventResponseWithDefaults

`func NewAssetEventResponseWithDefaults() *AssetEventResponse`

NewAssetEventResponseWithDefaults instantiates a new AssetEventResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AssetEventResponse) GetId() int32`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AssetEventResponse) GetIdOk() (*int32, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AssetEventResponse) SetId(v int32)`

SetId sets Id field to given value.


### GetAssetId

`func (o *AssetEventResponse) GetAssetId() int32`

GetAssetId returns the AssetId field if non-nil, zero value otherwise.

### GetAssetIdOk

`func (o *AssetEventResponse) GetAssetIdOk() (*int32, bool)`

GetAssetIdOk returns a tuple with the AssetId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssetId

`func (o *AssetEventResponse) SetAssetId(v int32)`

SetAssetId sets AssetId field to given value.


### GetUri

`func (o *AssetEventResponse) GetUri() string`

GetUri returns the Uri field if non-nil, zero value otherwise.

### GetUriOk

`func (o *AssetEventResponse) GetUriOk() (*string, bool)`

GetUriOk returns a tuple with the Uri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUri

`func (o *AssetEventResponse) SetUri(v string)`

SetUri sets Uri field to given value.

### HasUri

`func (o *AssetEventResponse) HasUri() bool`

HasUri returns a boolean if a field has been set.

### GetName

`func (o *AssetEventResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AssetEventResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AssetEventResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *AssetEventResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetGroup

`func (o *AssetEventResponse) GetGroup() string`

GetGroup returns the Group field if non-nil, zero value otherwise.

### GetGroupOk

`func (o *AssetEventResponse) GetGroupOk() (*string, bool)`

GetGroupOk returns a tuple with the Group field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroup

`func (o *AssetEventResponse) SetGroup(v string)`

SetGroup sets Group field to given value.

### HasGroup

`func (o *AssetEventResponse) HasGroup() bool`

HasGroup returns a boolean if a field has been set.

### GetExtra

`func (o *AssetEventResponse) GetExtra() map[string]*interface{}`

GetExtra returns the Extra field if non-nil, zero value otherwise.

### GetExtraOk

`func (o *AssetEventResponse) GetExtraOk() (*map[string]*interface{}, bool)`

GetExtraOk returns a tuple with the Extra field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtra

`func (o *AssetEventResponse) SetExtra(v map[string]*interface{})`

SetExtra sets Extra field to given value.

### HasExtra

`func (o *AssetEventResponse) HasExtra() bool`

HasExtra returns a boolean if a field has been set.

### GetSourceTaskId

`func (o *AssetEventResponse) GetSourceTaskId() string`

GetSourceTaskId returns the SourceTaskId field if non-nil, zero value otherwise.

### GetSourceTaskIdOk

`func (o *AssetEventResponse) GetSourceTaskIdOk() (*string, bool)`

GetSourceTaskIdOk returns a tuple with the SourceTaskId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceTaskId

`func (o *AssetEventResponse) SetSourceTaskId(v string)`

SetSourceTaskId sets SourceTaskId field to given value.

### HasSourceTaskId

`func (o *AssetEventResponse) HasSourceTaskId() bool`

HasSourceTaskId returns a boolean if a field has been set.

### GetSourceDagId

`func (o *AssetEventResponse) GetSourceDagId() string`

GetSourceDagId returns the SourceDagId field if non-nil, zero value otherwise.

### GetSourceDagIdOk

`func (o *AssetEventResponse) GetSourceDagIdOk() (*string, bool)`

GetSourceDagIdOk returns a tuple with the SourceDagId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceDagId

`func (o *AssetEventResponse) SetSourceDagId(v string)`

SetSourceDagId sets SourceDagId field to given value.

### HasSourceDagId

`func (o *AssetEventResponse) HasSourceDagId() bool`

HasSourceDagId returns a boolean if a field has been set.

### GetSourceRunId

`func (o *AssetEventResponse) GetSourceRunId() string`

GetSourceRunId returns the SourceRunId field if non-nil, zero value otherwise.

### GetSourceRunIdOk

`func (o *AssetEventResponse) GetSourceRunIdOk() (*string, bool)`

GetSourceRunIdOk returns a tuple with the SourceRunId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceRunId

`func (o *AssetEventResponse) SetSourceRunId(v string)`

SetSourceRunId sets SourceRunId field to given value.

### HasSourceRunId

`func (o *AssetEventResponse) HasSourceRunId() bool`

HasSourceRunId returns a boolean if a field has been set.

### GetSourceMapIndex

`func (o *AssetEventResponse) GetSourceMapIndex() int32`

GetSourceMapIndex returns the SourceMapIndex field if non-nil, zero value otherwise.

### GetSourceMapIndexOk

`func (o *AssetEventResponse) GetSourceMapIndexOk() (*int32, bool)`

GetSourceMapIndexOk returns a tuple with the SourceMapIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceMapIndex

`func (o *AssetEventResponse) SetSourceMapIndex(v int32)`

SetSourceMapIndex sets SourceMapIndex field to given value.


### GetCreatedDagruns

`func (o *AssetEventResponse) GetCreatedDagruns() []DagRunAssetReference`

GetCreatedDagruns returns the CreatedDagruns field if non-nil, zero value otherwise.

### GetCreatedDagrunsOk

`func (o *AssetEventResponse) GetCreatedDagrunsOk() (*[]DagRunAssetReference, bool)`

GetCreatedDagrunsOk returns a tuple with the CreatedDagruns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedDagruns

`func (o *AssetEventResponse) SetCreatedDagruns(v []DagRunAssetReference)`

SetCreatedDagruns sets CreatedDagruns field to given value.


### GetTimestamp

`func (o *AssetEventResponse) GetTimestamp() time.Time`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *AssetEventResponse) GetTimestampOk() (*time.Time, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *AssetEventResponse) SetTimestamp(v time.Time)`

SetTimestamp sets Timestamp field to given value.


### GetPartitionKey

`func (o *AssetEventResponse) GetPartitionKey() string`

GetPartitionKey returns the PartitionKey field if non-nil, zero value otherwise.

### GetPartitionKeyOk

`func (o *AssetEventResponse) GetPartitionKeyOk() (*string, bool)`

GetPartitionKeyOk returns a tuple with the PartitionKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartitionKey

`func (o *AssetEventResponse) SetPartitionKey(v string)`

SetPartitionKey sets PartitionKey field to given value.

### HasPartitionKey

`func (o *AssetEventResponse) HasPartitionKey() bool`

HasPartitionKey returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


