# HITLDetailResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**RespondedBy** | [**HITLUser**](HITLUser.md) |  | 
**RespondedAt** | **time.Time** |  | 
**ChosenOptions** | **[]string** |  | 
**ParamsInput** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewHITLDetailResponse

`func NewHITLDetailResponse(respondedBy HITLUser, respondedAt time.Time, chosenOptions []string, ) *HITLDetailResponse`

NewHITLDetailResponse instantiates a new HITLDetailResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewHITLDetailResponseWithDefaults

`func NewHITLDetailResponseWithDefaults() *HITLDetailResponse`

NewHITLDetailResponseWithDefaults instantiates a new HITLDetailResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRespondedBy

`func (o *HITLDetailResponse) GetRespondedBy() HITLUser`

GetRespondedBy returns the RespondedBy field if non-nil, zero value otherwise.

### GetRespondedByOk

`func (o *HITLDetailResponse) GetRespondedByOk() (*HITLUser, bool)`

GetRespondedByOk returns a tuple with the RespondedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRespondedBy

`func (o *HITLDetailResponse) SetRespondedBy(v HITLUser)`

SetRespondedBy sets RespondedBy field to given value.


### GetRespondedAt

`func (o *HITLDetailResponse) GetRespondedAt() time.Time`

GetRespondedAt returns the RespondedAt field if non-nil, zero value otherwise.

### GetRespondedAtOk

`func (o *HITLDetailResponse) GetRespondedAtOk() (*time.Time, bool)`

GetRespondedAtOk returns a tuple with the RespondedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRespondedAt

`func (o *HITLDetailResponse) SetRespondedAt(v time.Time)`

SetRespondedAt sets RespondedAt field to given value.


### GetChosenOptions

`func (o *HITLDetailResponse) GetChosenOptions() []string`

GetChosenOptions returns the ChosenOptions field if non-nil, zero value otherwise.

### GetChosenOptionsOk

`func (o *HITLDetailResponse) GetChosenOptionsOk() (*[]string, bool)`

GetChosenOptionsOk returns a tuple with the ChosenOptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChosenOptions

`func (o *HITLDetailResponse) SetChosenOptions(v []string)`

SetChosenOptions sets ChosenOptions field to given value.


### GetParamsInput

`func (o *HITLDetailResponse) GetParamsInput() map[string]interface{}`

GetParamsInput returns the ParamsInput field if non-nil, zero value otherwise.

### GetParamsInputOk

`func (o *HITLDetailResponse) GetParamsInputOk() (*map[string]interface{}, bool)`

GetParamsInputOk returns a tuple with the ParamsInput field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParamsInput

`func (o *HITLDetailResponse) SetParamsInput(v map[string]interface{})`

SetParamsInput sets ParamsInput field to given value.

### HasParamsInput

`func (o *HITLDetailResponse) HasParamsInput() bool`

HasParamsInput returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


