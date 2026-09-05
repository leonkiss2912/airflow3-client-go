# CreateAssetEventsBody

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AssetId** | **int32** |  | 
**PartitionKey** | Pointer to **NullableString** |  | [optional] 
**Extra** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewCreateAssetEventsBody

`func NewCreateAssetEventsBody(assetId int32, ) *CreateAssetEventsBody`

NewCreateAssetEventsBody instantiates a new CreateAssetEventsBody object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateAssetEventsBodyWithDefaults

`func NewCreateAssetEventsBodyWithDefaults() *CreateAssetEventsBody`

NewCreateAssetEventsBodyWithDefaults instantiates a new CreateAssetEventsBody object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAssetId

`func (o *CreateAssetEventsBody) GetAssetId() int32`

GetAssetId returns the AssetId field if non-nil, zero value otherwise.

### GetAssetIdOk

`func (o *CreateAssetEventsBody) GetAssetIdOk() (*int32, bool)`

GetAssetIdOk returns a tuple with the AssetId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssetId

`func (o *CreateAssetEventsBody) SetAssetId(v int32)`

SetAssetId sets AssetId field to given value.


### GetPartitionKey

`func (o *CreateAssetEventsBody) GetPartitionKey() string`

GetPartitionKey returns the PartitionKey field if non-nil, zero value otherwise.

### GetPartitionKeyOk

`func (o *CreateAssetEventsBody) GetPartitionKeyOk() (*string, bool)`

GetPartitionKeyOk returns a tuple with the PartitionKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPartitionKey

`func (o *CreateAssetEventsBody) SetPartitionKey(v string)`

SetPartitionKey sets PartitionKey field to given value.

### HasPartitionKey

`func (o *CreateAssetEventsBody) HasPartitionKey() bool`

HasPartitionKey returns a boolean if a field has been set.

### SetPartitionKeyNil

`func (o *CreateAssetEventsBody) SetPartitionKeyNil(b bool)`

 SetPartitionKeyNil sets the value for PartitionKey to be an explicit nil

### UnsetPartitionKey
`func (o *CreateAssetEventsBody) UnsetPartitionKey()`

UnsetPartitionKey ensures that no value is present for PartitionKey, not even an explicit nil
### GetExtra

`func (o *CreateAssetEventsBody) GetExtra() map[string]interface{}`

GetExtra returns the Extra field if non-nil, zero value otherwise.

### GetExtraOk

`func (o *CreateAssetEventsBody) GetExtraOk() (*map[string]interface{}, bool)`

GetExtraOk returns a tuple with the Extra field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtra

`func (o *CreateAssetEventsBody) SetExtra(v map[string]interface{})`

SetExtra sets Extra field to given value.

### HasExtra

`func (o *CreateAssetEventsBody) HasExtra() bool`

HasExtra returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


