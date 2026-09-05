# AssetWatcherResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**TriggerId** | **int32** |  | 
**CreatedDate** | **time.Time** |  | 

## Methods

### NewAssetWatcherResponse

`func NewAssetWatcherResponse(name string, triggerId int32, createdDate time.Time, ) *AssetWatcherResponse`

NewAssetWatcherResponse instantiates a new AssetWatcherResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAssetWatcherResponseWithDefaults

`func NewAssetWatcherResponseWithDefaults() *AssetWatcherResponse`

NewAssetWatcherResponseWithDefaults instantiates a new AssetWatcherResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *AssetWatcherResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AssetWatcherResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AssetWatcherResponse) SetName(v string)`

SetName sets Name field to given value.


### GetTriggerId

`func (o *AssetWatcherResponse) GetTriggerId() int32`

GetTriggerId returns the TriggerId field if non-nil, zero value otherwise.

### GetTriggerIdOk

`func (o *AssetWatcherResponse) GetTriggerIdOk() (*int32, bool)`

GetTriggerIdOk returns a tuple with the TriggerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTriggerId

`func (o *AssetWatcherResponse) SetTriggerId(v int32)`

SetTriggerId sets TriggerId field to given value.


### GetCreatedDate

`func (o *AssetWatcherResponse) GetCreatedDate() time.Time`

GetCreatedDate returns the CreatedDate field if non-nil, zero value otherwise.

### GetCreatedDateOk

`func (o *AssetWatcherResponse) GetCreatedDateOk() (*time.Time, bool)`

GetCreatedDateOk returns a tuple with the CreatedDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedDate

`func (o *AssetWatcherResponse) SetCreatedDate(v time.Time)`

SetCreatedDate sets CreatedDate field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


