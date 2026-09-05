# \JobAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetJobs**](JobAPI.md#GetJobs) | **Get** /api/v2/jobs | Get Jobs



## GetJobs

> JobCollectionResponse GetJobs(ctx).IsAlive(isAlive).StartDateGte(startDateGte).StartDateGt(startDateGt).StartDateLte(startDateLte).StartDateLt(startDateLt).EndDateGte(endDateGte).EndDateGt(endDateGt).EndDateLte(endDateLte).EndDateLt(endDateLt).Limit(limit).Offset(offset).OrderBy(orderBy).JobState(jobState).JobType(jobType).Hostname(hostname).ExecutorClass(executorClass).Execute()

Get Jobs



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	isAlive := true // bool |  (optional)
	startDateGte := time.Now() // time.Time |  (optional)
	startDateGt := time.Now() // time.Time |  (optional)
	startDateLte := time.Now() // time.Time |  (optional)
	startDateLt := time.Now() // time.Time |  (optional)
	endDateGte := time.Now() // time.Time |  (optional)
	endDateGt := time.Now() // time.Time |  (optional)
	endDateLte := time.Now() // time.Time |  (optional)
	endDateLt := time.Now() // time.Time |  (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	orderBy := []*string{"Inner_example"} // []*string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `id, dag_id, state, job_type, start_date, end_date, latest_heartbeat, executor_class, hostname, unixname` (optional) (default to {"id"})
	jobState := "jobState_example" // string |  (optional)
	jobType := "jobType_example" // string |  (optional)
	hostname := "hostname_example" // string |  (optional)
	executorClass := "executorClass_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.JobAPI.GetJobs(context.Background()).IsAlive(isAlive).StartDateGte(startDateGte).StartDateGt(startDateGt).StartDateLte(startDateLte).StartDateLt(startDateLt).EndDateGte(endDateGte).EndDateGt(endDateGt).EndDateLte(endDateLte).EndDateLt(endDateLt).Limit(limit).Offset(offset).OrderBy(orderBy).JobState(jobState).JobType(jobType).Hostname(hostname).ExecutorClass(executorClass).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `JobAPI.GetJobs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetJobs`: JobCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `JobAPI.GetJobs`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetJobsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **isAlive** | **bool** |  | 
 **startDateGte** | **time.Time** |  | 
 **startDateGt** | **time.Time** |  | 
 **startDateLte** | **time.Time** |  | 
 **startDateLt** | **time.Time** |  | 
 **endDateGte** | **time.Time** |  | 
 **endDateGt** | **time.Time** |  | 
 **endDateLte** | **time.Time** |  | 
 **endDateLt** | **time.Time** |  | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;id, dag_id, state, job_type, start_date, end_date, latest_heartbeat, executor_class, hostname, unixname&#x60; | [default to {&quot;id&quot;}]
 **jobState** | **string** |  | 
 **jobType** | **string** |  | 
 **hostname** | **string** |  | 
 **executorClass** | **string** |  | 

### Return type

[**JobCollectionResponse**](JobCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

