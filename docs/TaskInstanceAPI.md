# \TaskInstanceAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BulkTaskInstances**](TaskInstanceAPI.md#BulkTaskInstances) | **Patch** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances | Bulk Task Instances
[**DeleteTaskInstance**](TaskInstanceAPI.md#DeleteTaskInstance) | **Delete** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id} | Delete Task Instance
[**GetExternalLogUrl**](TaskInstanceAPI.md#GetExternalLogUrl) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/externalLogUrl/{try_number} | Get External Log Url
[**GetExtraLinks**](TaskInstanceAPI.md#GetExtraLinks) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/links | Get Extra Links
[**GetHitlDetail**](TaskInstanceAPI.md#GetHitlDetail) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/{map_index}/hitlDetails | Get Hitl Detail
[**GetHitlDetailTryDetail**](TaskInstanceAPI.md#GetHitlDetailTryDetail) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/{map_index}/hitlDetails/tries/{try_number} | Get Hitl Detail Try Detail
[**GetHitlDetails**](TaskInstanceAPI.md#GetHitlDetails) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/hitlDetails | Get Hitl Details
[**GetLog**](TaskInstanceAPI.md#GetLog) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/logs/{try_number} | Get Log
[**GetMappedTaskInstance**](TaskInstanceAPI.md#GetMappedTaskInstance) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/{map_index} | Get Mapped Task Instance
[**GetMappedTaskInstanceTries**](TaskInstanceAPI.md#GetMappedTaskInstanceTries) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/{map_index}/tries | Get Mapped Task Instance Tries
[**GetMappedTaskInstanceTryDetails**](TaskInstanceAPI.md#GetMappedTaskInstanceTryDetails) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/{map_index}/tries/{task_try_number} | Get Mapped Task Instance Try Details
[**GetMappedTaskInstances**](TaskInstanceAPI.md#GetMappedTaskInstances) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/listMapped | Get Mapped Task Instances
[**GetTaskInstance**](TaskInstanceAPI.md#GetTaskInstance) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id} | Get Task Instance
[**GetTaskInstanceDependencies**](TaskInstanceAPI.md#GetTaskInstanceDependencies) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/dependencies | Get Task Instance Dependencies
[**GetTaskInstanceDependenciesByMapIndex**](TaskInstanceAPI.md#GetTaskInstanceDependenciesByMapIndex) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/{map_index}/dependencies | Get Task Instance Dependencies
[**GetTaskInstanceTries**](TaskInstanceAPI.md#GetTaskInstanceTries) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/tries | Get Task Instance Tries
[**GetTaskInstanceTryDetails**](TaskInstanceAPI.md#GetTaskInstanceTryDetails) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/tries/{task_try_number} | Get Task Instance Try Details
[**GetTaskInstances**](TaskInstanceAPI.md#GetTaskInstances) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances | Get Task Instances
[**GetTaskInstancesBatch**](TaskInstanceAPI.md#GetTaskInstancesBatch) | **Post** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/list | Get Task Instances Batch
[**PatchTaskInstance**](TaskInstanceAPI.md#PatchTaskInstance) | **Patch** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id} | Patch Task Instance
[**PatchTaskInstanceByMapIndex**](TaskInstanceAPI.md#PatchTaskInstanceByMapIndex) | **Patch** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/{map_index} | Patch Task Instance
[**PatchTaskInstanceDryRun**](TaskInstanceAPI.md#PatchTaskInstanceDryRun) | **Patch** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/dry_run | Patch Task Instance Dry Run
[**PatchTaskInstanceDryRunByMapIndex**](TaskInstanceAPI.md#PatchTaskInstanceDryRunByMapIndex) | **Patch** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/{map_index}/dry_run | Patch Task Instance Dry Run
[**PostClearTaskInstances**](TaskInstanceAPI.md#PostClearTaskInstances) | **Post** /api/v2/dags/{dag_id}/clearTaskInstances | Post Clear Task Instances
[**UpdateHitlDetail**](TaskInstanceAPI.md#UpdateHitlDetail) | **Patch** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/{map_index}/hitlDetails | Update Hitl Detail



## BulkTaskInstances

> BulkResponse BulkTaskInstances(ctx, dagId, dagRunId).BulkBodyBulkTaskInstanceBody(bulkBodyBulkTaskInstanceBody).Execute()

Bulk Task Instances



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	bulkBodyBulkTaskInstanceBody := *openapiclient.NewBulkBodyBulkTaskInstanceBody([]openapiclient.ActionsInner{openapiclient.Actions_inner{BulkCreateActionBulkTaskInstanceBody: openapiclient.NewBulkCreateActionBulkTaskInstanceBody("Action_example", []openapiclient.BulkTaskInstanceBody{*openapiclient.NewBulkTaskInstanceBody("TaskId_example")})}}) // BulkBodyBulkTaskInstanceBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.BulkTaskInstances(context.Background(), dagId, dagRunId).BulkBodyBulkTaskInstanceBody(bulkBodyBulkTaskInstanceBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.BulkTaskInstances``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BulkTaskInstances`: BulkResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.BulkTaskInstances`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiBulkTaskInstancesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **bulkBodyBulkTaskInstanceBody** | [**BulkBodyBulkTaskInstanceBody**](BulkBodyBulkTaskInstanceBody.md) |  | 

### Return type

[**BulkResponse**](BulkResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteTaskInstance

> interface{} DeleteTaskInstance(ctx, dagId, dagRunId, taskId).MapIndex(mapIndex).Execute()

Delete Task Instance



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 |  (optional) (default to -1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.DeleteTaskInstance(context.Background(), dagId, dagRunId, taskId).MapIndex(mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.DeleteTaskInstance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteTaskInstance`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.DeleteTaskInstance`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTaskInstanceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **mapIndex** | **int32** |  | [default to -1]

### Return type

**interface{}**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetExternalLogUrl

> ExternalLogUrlResponse GetExternalLogUrl(ctx, dagId, dagRunId, taskId, tryNumber).MapIndex(mapIndex).Execute()

Get External Log Url



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	tryNumber := int32(56) // int32 | 
	mapIndex := int32(56) // int32 |  (optional) (default to -1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetExternalLogUrl(context.Background(), dagId, dagRunId, taskId, tryNumber).MapIndex(mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetExternalLogUrl``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetExternalLogUrl`: ExternalLogUrlResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetExternalLogUrl`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**tryNumber** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetExternalLogUrlRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **mapIndex** | **int32** |  | [default to -1]

### Return type

[**ExternalLogUrlResponse**](ExternalLogUrlResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetExtraLinks

> ExtraLinkCollectionResponse GetExtraLinks(ctx, dagId, dagRunId, taskId).MapIndex(mapIndex).TryNumber(tryNumber).Execute()

Get Extra Links



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 |  (optional) (default to -1)
	tryNumber := int32(56) // int32 |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetExtraLinks(context.Background(), dagId, dagRunId, taskId).MapIndex(mapIndex).TryNumber(tryNumber).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetExtraLinks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetExtraLinks`: ExtraLinkCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetExtraLinks`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetExtraLinksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **mapIndex** | **int32** |  | [default to -1]
 **tryNumber** | **int32** |  | 

### Return type

[**ExtraLinkCollectionResponse**](ExtraLinkCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetHitlDetail

> HITLDetail GetHitlDetail(ctx, dagId, dagRunId, taskId, mapIndex).Execute()

Get Hitl Detail



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetHitlDetail(context.Background(), dagId, dagRunId, taskId, mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetHitlDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetHitlDetail`: HITLDetail
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetHitlDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**mapIndex** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetHitlDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------





### Return type

[**HITLDetail**](HITLDetail.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetHitlDetailTryDetail

> HITLDetailHistory GetHitlDetailTryDetail(ctx, dagId, dagRunId, taskId, mapIndex, tryNumber).Execute()

Get Hitl Detail Try Detail



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 | 
	tryNumber := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetHitlDetailTryDetail(context.Background(), dagId, dagRunId, taskId, mapIndex, tryNumber).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetHitlDetailTryDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetHitlDetailTryDetail`: HITLDetailHistory
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetHitlDetailTryDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**mapIndex** | **int32** |  | 
**tryNumber** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetHitlDetailTryDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------






### Return type

[**HITLDetailHistory**](HITLDetailHistory.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetHitlDetails

> HITLDetailCollection GetHitlDetails(ctx, dagId, dagRunId).Limit(limit).Offset(offset).OrderBy(orderBy).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).TaskId(taskId).TaskIdPattern(taskIdPattern).TaskIdPrefixPattern(taskIdPrefixPattern).MapIndex(mapIndex).State(state).ResponseReceived(responseReceived).RespondedByUserId(respondedByUserId).RespondedByUserName(respondedByUserName).SubjectSearch(subjectSearch).BodySearch(bodySearch).CreatedAtGte(createdAtGte).CreatedAtGt(createdAtGt).CreatedAtLte(createdAtLte).CreatedAtLt(createdAtLt).Execute()

Get Hitl Details



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	orderBy := []string{"Inner_example"} // []string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `ti_id, subject, responded_at, created_at, responded_by_user_id, responded_by_user_name, dag_id, run_id, task_display_name, run_after, rendered_map_index, task_instance_operator, task_instance_state` (optional) (default to {"ti_id"})
	dagIdPattern := "dagIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``dag_id_prefix_pattern`` parameter when possible. (optional)
	dagIdPrefixPattern := "dagIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	taskId := "taskId_example" // string |  (optional)
	taskIdPattern := "taskIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``task_id_prefix_pattern`` parameter when possible. (optional)
	taskIdPrefixPattern := "taskIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	mapIndex := int32(56) // int32 |  (optional)
	state := []string{"Inner_example"} // []string |  (optional)
	responseReceived := true // bool |  (optional)
	respondedByUserId := []string{"Inner_example"} // []string |  (optional)
	respondedByUserName := []string{"Inner_example"} // []string |  (optional)
	subjectSearch := "subjectSearch_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``subject_search`` parameter when possible. (optional)
	bodySearch := "bodySearch_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``body_search`` parameter when possible. (optional)
	createdAtGte := time.Now() // time.Time |  (optional)
	createdAtGt := time.Now() // time.Time |  (optional)
	createdAtLte := time.Now() // time.Time |  (optional)
	createdAtLt := time.Now() // time.Time |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetHitlDetails(context.Background(), dagId, dagRunId).Limit(limit).Offset(offset).OrderBy(orderBy).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).TaskId(taskId).TaskIdPattern(taskIdPattern).TaskIdPrefixPattern(taskIdPrefixPattern).MapIndex(mapIndex).State(state).ResponseReceived(responseReceived).RespondedByUserId(respondedByUserId).RespondedByUserName(respondedByUserName).SubjectSearch(subjectSearch).BodySearch(bodySearch).CreatedAtGte(createdAtGte).CreatedAtGt(createdAtGt).CreatedAtLte(createdAtLte).CreatedAtLt(createdAtLt).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetHitlDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetHitlDetails`: HITLDetailCollection
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetHitlDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetHitlDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;ti_id, subject, responded_at, created_at, responded_by_user_id, responded_by_user_name, dag_id, run_id, task_display_name, run_after, rendered_map_index, task_instance_operator, task_instance_state&#x60; | [default to {&quot;ti_id&quot;}]
 **dagIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;dag_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **dagIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **taskId** | **string** |  | 
 **taskIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;task_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **taskIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **mapIndex** | **int32** |  | 
 **state** | **[]string** |  | 
 **responseReceived** | **bool** |  | 
 **respondedByUserId** | **[]string** |  | 
 **respondedByUserName** | **[]string** |  | 
 **subjectSearch** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;subject_search&#x60;&#x60; parameter when possible. | 
 **bodySearch** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;body_search&#x60;&#x60; parameter when possible. | 
 **createdAtGte** | **time.Time** |  | 
 **createdAtGt** | **time.Time** |  | 
 **createdAtLte** | **time.Time** |  | 
 **createdAtLt** | **time.Time** |  | 

### Return type

[**HITLDetailCollection**](HITLDetailCollection.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetLog

> TaskInstancesLogResponse GetLog(ctx, dagId, dagRunId, taskId, tryNumber).FullContent(fullContent).MapIndex(mapIndex).Token(token).Accept(accept).Execute()

Get Log



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	tryNumber := int32(56) // int32 | 
	fullContent := true // bool |  (optional) (default to false)
	mapIndex := int32(56) // int32 |  (optional) (default to -1)
	token := "token_example" // string |  (optional)
	accept := "accept_example" // string |  (optional) (default to "*_/_*")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetLog(context.Background(), dagId, dagRunId, taskId, tryNumber).FullContent(fullContent).MapIndex(mapIndex).Token(token).Accept(accept).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetLog``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetLog`: TaskInstancesLogResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetLog`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**tryNumber** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetLogRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **fullContent** | **bool** |  | [default to false]
 **mapIndex** | **int32** |  | [default to -1]
 **token** | **string** |  | 
 **accept** | **string** |  | [default to &quot;*_/_*&quot;]

### Return type

[**TaskInstancesLogResponse**](TaskInstancesLogResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/x-ndjson

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMappedTaskInstance

> TaskInstanceResponse GetMappedTaskInstance(ctx, dagId, dagRunId, taskId, mapIndex).Execute()

Get Mapped Task Instance



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetMappedTaskInstance(context.Background(), dagId, dagRunId, taskId, mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetMappedTaskInstance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMappedTaskInstance`: TaskInstanceResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetMappedTaskInstance`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**mapIndex** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMappedTaskInstanceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------





### Return type

[**TaskInstanceResponse**](TaskInstanceResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMappedTaskInstanceTries

> TaskInstanceHistoryCollectionResponse GetMappedTaskInstanceTries(ctx, dagId, dagRunId, taskId, mapIndex).Execute()

Get Mapped Task Instance Tries

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetMappedTaskInstanceTries(context.Background(), dagId, dagRunId, taskId, mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetMappedTaskInstanceTries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMappedTaskInstanceTries`: TaskInstanceHistoryCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetMappedTaskInstanceTries`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**mapIndex** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMappedTaskInstanceTriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------





### Return type

[**TaskInstanceHistoryCollectionResponse**](TaskInstanceHistoryCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMappedTaskInstanceTryDetails

> TaskInstanceHistoryResponse GetMappedTaskInstanceTryDetails(ctx, dagId, dagRunId, taskId, taskTryNumber, mapIndex).Execute()

Get Mapped Task Instance Try Details

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	taskTryNumber := int32(56) // int32 | 
	mapIndex := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetMappedTaskInstanceTryDetails(context.Background(), dagId, dagRunId, taskId, taskTryNumber, mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetMappedTaskInstanceTryDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMappedTaskInstanceTryDetails`: TaskInstanceHistoryResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetMappedTaskInstanceTryDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**taskTryNumber** | **int32** |  | 
**mapIndex** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMappedTaskInstanceTryDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------






### Return type

[**TaskInstanceHistoryResponse**](TaskInstanceHistoryResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMappedTaskInstances

> TaskInstanceCollectionResponse GetMappedTaskInstances(ctx, dagId, dagRunId, taskId).RunAfterGte(runAfterGte).RunAfterGt(runAfterGt).RunAfterLte(runAfterLte).RunAfterLt(runAfterLt).LogicalDateGte(logicalDateGte).LogicalDateGt(logicalDateGt).LogicalDateLte(logicalDateLte).LogicalDateLt(logicalDateLt).StartDateGte(startDateGte).StartDateGt(startDateGt).StartDateLte(startDateLte).StartDateLt(startDateLt).EndDateGte(endDateGte).EndDateGt(endDateGt).EndDateLte(endDateLte).EndDateLt(endDateLt).UpdatedAtGte(updatedAtGte).UpdatedAtGt(updatedAtGt).UpdatedAtLte(updatedAtLte).UpdatedAtLt(updatedAtLt).DurationGte(durationGte).DurationGt(durationGt).DurationLte(durationLte).DurationLt(durationLt).State(state).Pool(pool).PoolNamePattern(poolNamePattern).PoolNamePrefixPattern(poolNamePrefixPattern).Queue(queue).QueueNamePattern(queueNamePattern).QueueNamePrefixPattern(queueNamePrefixPattern).Executor(executor).VersionNumber(versionNumber).TryNumber(tryNumber).Operator(operator).OperatorNamePattern(operatorNamePattern).OperatorNamePrefixPattern(operatorNamePrefixPattern).MapIndex(mapIndex).RenderedMapIndexPattern(renderedMapIndexPattern).RenderedMapIndexPrefixPattern(renderedMapIndexPrefixPattern).Limit(limit).Offset(offset).OrderBy(orderBy).Execute()

Get Mapped Task Instances



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	runAfterGte := time.Now() // time.Time |  (optional)
	runAfterGt := time.Now() // time.Time |  (optional)
	runAfterLte := time.Now() // time.Time |  (optional)
	runAfterLt := time.Now() // time.Time |  (optional)
	logicalDateGte := time.Now() // time.Time |  (optional)
	logicalDateGt := time.Now() // time.Time |  (optional)
	logicalDateLte := time.Now() // time.Time |  (optional)
	logicalDateLt := time.Now() // time.Time |  (optional)
	startDateGte := time.Now() // time.Time |  (optional)
	startDateGt := time.Now() // time.Time |  (optional)
	startDateLte := time.Now() // time.Time |  (optional)
	startDateLt := time.Now() // time.Time |  (optional)
	endDateGte := time.Now() // time.Time |  (optional)
	endDateGt := time.Now() // time.Time |  (optional)
	endDateLte := time.Now() // time.Time |  (optional)
	endDateLt := time.Now() // time.Time |  (optional)
	updatedAtGte := time.Now() // time.Time |  (optional)
	updatedAtGt := time.Now() // time.Time |  (optional)
	updatedAtLte := time.Now() // time.Time |  (optional)
	updatedAtLt := time.Now() // time.Time |  (optional)
	durationGte := float32(8.14) // float32 |  (optional)
	durationGt := float32(8.14) // float32 |  (optional)
	durationLte := float32(8.14) // float32 |  (optional)
	durationLt := float32(8.14) // float32 |  (optional)
	state := []string{"Inner_example"} // []string |  (optional)
	pool := []string{"Inner_example"} // []string |  (optional)
	poolNamePattern := "poolNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``pool_name_prefix_pattern`` parameter when possible. (optional)
	poolNamePrefixPattern := "poolNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	queue := []string{"Inner_example"} // []string |  (optional)
	queueNamePattern := "queueNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``queue_name_prefix_pattern`` parameter when possible. (optional)
	queueNamePrefixPattern := "queueNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	executor := []string{"Inner_example"} // []string |  (optional)
	versionNumber := []int32{int32(123)} // []int32 |  (optional)
	tryNumber := []int32{int32(123)} // []int32 |  (optional)
	operator := []string{"Inner_example"} // []string |  (optional)
	operatorNamePattern := "operatorNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``operator_name_prefix_pattern`` parameter when possible. (optional)
	operatorNamePrefixPattern := "operatorNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	mapIndex := []int32{int32(123)} // []int32 |  (optional)
	renderedMapIndexPattern := "renderedMapIndexPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``rendered_map_index_prefix_pattern`` parameter when possible. (optional)
	renderedMapIndexPrefixPattern := "renderedMapIndexPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	orderBy := []string{"Inner_example"} // []string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `id, state, duration, start_date, end_date, map_index, try_number, logical_date, run_after, data_interval_start, data_interval_end, rendered_map_index, operator, run_after, logical_date, data_interval_start, data_interval_end` (optional) (default to {"map_index"})

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetMappedTaskInstances(context.Background(), dagId, dagRunId, taskId).RunAfterGte(runAfterGte).RunAfterGt(runAfterGt).RunAfterLte(runAfterLte).RunAfterLt(runAfterLt).LogicalDateGte(logicalDateGte).LogicalDateGt(logicalDateGt).LogicalDateLte(logicalDateLte).LogicalDateLt(logicalDateLt).StartDateGte(startDateGte).StartDateGt(startDateGt).StartDateLte(startDateLte).StartDateLt(startDateLt).EndDateGte(endDateGte).EndDateGt(endDateGt).EndDateLte(endDateLte).EndDateLt(endDateLt).UpdatedAtGte(updatedAtGte).UpdatedAtGt(updatedAtGt).UpdatedAtLte(updatedAtLte).UpdatedAtLt(updatedAtLt).DurationGte(durationGte).DurationGt(durationGt).DurationLte(durationLte).DurationLt(durationLt).State(state).Pool(pool).PoolNamePattern(poolNamePattern).PoolNamePrefixPattern(poolNamePrefixPattern).Queue(queue).QueueNamePattern(queueNamePattern).QueueNamePrefixPattern(queueNamePrefixPattern).Executor(executor).VersionNumber(versionNumber).TryNumber(tryNumber).Operator(operator).OperatorNamePattern(operatorNamePattern).OperatorNamePrefixPattern(operatorNamePrefixPattern).MapIndex(mapIndex).RenderedMapIndexPattern(renderedMapIndexPattern).RenderedMapIndexPrefixPattern(renderedMapIndexPrefixPattern).Limit(limit).Offset(offset).OrderBy(orderBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetMappedTaskInstances``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMappedTaskInstances`: TaskInstanceCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetMappedTaskInstances`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMappedTaskInstancesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **runAfterGte** | **time.Time** |  | 
 **runAfterGt** | **time.Time** |  | 
 **runAfterLte** | **time.Time** |  | 
 **runAfterLt** | **time.Time** |  | 
 **logicalDateGte** | **time.Time** |  | 
 **logicalDateGt** | **time.Time** |  | 
 **logicalDateLte** | **time.Time** |  | 
 **logicalDateLt** | **time.Time** |  | 
 **startDateGte** | **time.Time** |  | 
 **startDateGt** | **time.Time** |  | 
 **startDateLte** | **time.Time** |  | 
 **startDateLt** | **time.Time** |  | 
 **endDateGte** | **time.Time** |  | 
 **endDateGt** | **time.Time** |  | 
 **endDateLte** | **time.Time** |  | 
 **endDateLt** | **time.Time** |  | 
 **updatedAtGte** | **time.Time** |  | 
 **updatedAtGt** | **time.Time** |  | 
 **updatedAtLte** | **time.Time** |  | 
 **updatedAtLt** | **time.Time** |  | 
 **durationGte** | **float32** |  | 
 **durationGt** | **float32** |  | 
 **durationLte** | **float32** |  | 
 **durationLt** | **float32** |  | 
 **state** | **[]string** |  | 
 **pool** | **[]string** |  | 
 **poolNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;pool_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **poolNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **queue** | **[]string** |  | 
 **queueNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;queue_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **queueNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **executor** | **[]string** |  | 
 **versionNumber** | **[]int32** |  | 
 **tryNumber** | **[]int32** |  | 
 **operator** | **[]string** |  | 
 **operatorNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;operator_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **operatorNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **mapIndex** | **[]int32** |  | 
 **renderedMapIndexPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;rendered_map_index_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **renderedMapIndexPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;id, state, duration, start_date, end_date, map_index, try_number, logical_date, run_after, data_interval_start, data_interval_end, rendered_map_index, operator, run_after, logical_date, data_interval_start, data_interval_end&#x60; | [default to {&quot;map_index&quot;}]

### Return type

[**TaskInstanceCollectionResponse**](TaskInstanceCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTaskInstance

> TaskInstanceResponse GetTaskInstance(ctx, dagId, dagRunId, taskId).Execute()

Get Task Instance



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetTaskInstance(context.Background(), dagId, dagRunId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetTaskInstance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTaskInstance`: TaskInstanceResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetTaskInstance`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaskInstanceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**TaskInstanceResponse**](TaskInstanceResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTaskInstanceDependencies

> TaskDependencyCollectionResponse GetTaskInstanceDependencies(ctx, dagId, dagRunId, taskId).MapIndex(mapIndex).Execute()

Get Task Instance Dependencies



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 |  (optional) (default to -1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetTaskInstanceDependencies(context.Background(), dagId, dagRunId, taskId).MapIndex(mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetTaskInstanceDependencies``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTaskInstanceDependencies`: TaskDependencyCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetTaskInstanceDependencies`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaskInstanceDependenciesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **mapIndex** | **int32** |  | [default to -1]

### Return type

[**TaskDependencyCollectionResponse**](TaskDependencyCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTaskInstanceDependenciesByMapIndex

> TaskDependencyCollectionResponse GetTaskInstanceDependenciesByMapIndex(ctx, dagId, dagRunId, taskId, mapIndex).Execute()

Get Task Instance Dependencies



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetTaskInstanceDependenciesByMapIndex(context.Background(), dagId, dagRunId, taskId, mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetTaskInstanceDependenciesByMapIndex``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTaskInstanceDependenciesByMapIndex`: TaskDependencyCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetTaskInstanceDependenciesByMapIndex`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**mapIndex** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaskInstanceDependenciesByMapIndexRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------





### Return type

[**TaskDependencyCollectionResponse**](TaskDependencyCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTaskInstanceTries

> TaskInstanceHistoryCollectionResponse GetTaskInstanceTries(ctx, dagId, dagRunId, taskId).MapIndex(mapIndex).Execute()

Get Task Instance Tries



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 |  (optional) (default to -1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetTaskInstanceTries(context.Background(), dagId, dagRunId, taskId).MapIndex(mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetTaskInstanceTries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTaskInstanceTries`: TaskInstanceHistoryCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetTaskInstanceTries`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaskInstanceTriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **mapIndex** | **int32** |  | [default to -1]

### Return type

[**TaskInstanceHistoryCollectionResponse**](TaskInstanceHistoryCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTaskInstanceTryDetails

> TaskInstanceHistoryResponse GetTaskInstanceTryDetails(ctx, dagId, dagRunId, taskId, taskTryNumber).MapIndex(mapIndex).Execute()

Get Task Instance Try Details



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	taskTryNumber := int32(56) // int32 | 
	mapIndex := int32(56) // int32 |  (optional) (default to -1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetTaskInstanceTryDetails(context.Background(), dagId, dagRunId, taskId, taskTryNumber).MapIndex(mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetTaskInstanceTryDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTaskInstanceTryDetails`: TaskInstanceHistoryResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetTaskInstanceTryDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**taskTryNumber** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaskInstanceTryDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **mapIndex** | **int32** |  | [default to -1]

### Return type

[**TaskInstanceHistoryResponse**](TaskInstanceHistoryResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTaskInstances

> TaskInstanceCollectionResponse GetTaskInstances(ctx, dagId, dagRunId).Cursor(cursor).TaskId(taskId).RunAfterGte(runAfterGte).RunAfterGt(runAfterGt).RunAfterLte(runAfterLte).RunAfterLt(runAfterLt).LogicalDateGte(logicalDateGte).LogicalDateGt(logicalDateGt).LogicalDateLte(logicalDateLte).LogicalDateLt(logicalDateLt).StartDateGte(startDateGte).StartDateGt(startDateGt).StartDateLte(startDateLte).StartDateLt(startDateLt).EndDateGte(endDateGte).EndDateGt(endDateGt).EndDateLte(endDateLte).EndDateLt(endDateLt).UpdatedAtGte(updatedAtGte).UpdatedAtGt(updatedAtGt).UpdatedAtLte(updatedAtLte).UpdatedAtLt(updatedAtLt).DurationGte(durationGte).DurationGt(durationGt).DurationLte(durationLte).DurationLt(durationLt).TaskDisplayNamePattern(taskDisplayNamePattern).TaskDisplayNamePrefixPattern(taskDisplayNamePrefixPattern).TaskGroupId(taskGroupId).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).RunIdPattern(runIdPattern).RunIdPrefixPattern(runIdPrefixPattern).State(state).Pool(pool).PoolNamePattern(poolNamePattern).PoolNamePrefixPattern(poolNamePrefixPattern).Queue(queue).QueueNamePattern(queueNamePattern).QueueNamePrefixPattern(queueNamePrefixPattern).Executor(executor).VersionNumber(versionNumber).TryNumber(tryNumber).Operator(operator).OperatorNamePattern(operatorNamePattern).OperatorNamePrefixPattern(operatorNamePrefixPattern).MapIndex(mapIndex).RenderedMapIndexPattern(renderedMapIndexPattern).RenderedMapIndexPrefixPattern(renderedMapIndexPrefixPattern).Limit(limit).Offset(offset).OrderBy(orderBy).Execute()

Get Task Instances



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	cursor := "cursor_example" // string | Cursor for keyset-based pagination. Pass an empty string for the first page, then use ``next_cursor`` from the response. When ``cursor`` is provided, ``offset`` is ignored. (optional)
	taskId := "taskId_example" // string |  (optional)
	runAfterGte := time.Now() // time.Time |  (optional)
	runAfterGt := time.Now() // time.Time |  (optional)
	runAfterLte := time.Now() // time.Time |  (optional)
	runAfterLt := time.Now() // time.Time |  (optional)
	logicalDateGte := time.Now() // time.Time |  (optional)
	logicalDateGt := time.Now() // time.Time |  (optional)
	logicalDateLte := time.Now() // time.Time |  (optional)
	logicalDateLt := time.Now() // time.Time |  (optional)
	startDateGte := time.Now() // time.Time |  (optional)
	startDateGt := time.Now() // time.Time |  (optional)
	startDateLte := time.Now() // time.Time |  (optional)
	startDateLt := time.Now() // time.Time |  (optional)
	endDateGte := time.Now() // time.Time |  (optional)
	endDateGt := time.Now() // time.Time |  (optional)
	endDateLte := time.Now() // time.Time |  (optional)
	endDateLt := time.Now() // time.Time |  (optional)
	updatedAtGte := time.Now() // time.Time |  (optional)
	updatedAtGt := time.Now() // time.Time |  (optional)
	updatedAtLte := time.Now() // time.Time |  (optional)
	updatedAtLt := time.Now() // time.Time |  (optional)
	durationGte := float32(8.14) // float32 |  (optional)
	durationGt := float32(8.14) // float32 |  (optional)
	durationLte := float32(8.14) // float32 |  (optional)
	durationLt := float32(8.14) // float32 |  (optional)
	taskDisplayNamePattern := "taskDisplayNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``task_display_name_prefix_pattern`` parameter when possible. (optional)
	taskDisplayNamePrefixPattern := "taskDisplayNamePrefixPattern_example" // string | Prefix match on task display name: optional ``_task_display_property_value`` else ``task_id`` (same as ``coalesce``). Case-sensitive. Index-friendly alternative to ``task_display_name_pattern``. On large databases, combine with ``dag_id_prefix_pattern`` (or a specific Dag in the path) so ``(dag_id, task_id, ...)`` indexes apply. Use ``|`` for OR. Use ``~`` to match all. Trailing non-alphanumeric characters in the term are stripped before matching so the range scan stays index-compatible under locale-aware collations. (optional)
	taskGroupId := "taskGroupId_example" // string | Filter by exact task group ID. Returns all tasks within the specified task group. (optional)
	dagIdPattern := "dagIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``dag_id_prefix_pattern`` parameter when possible. (optional)
	dagIdPrefixPattern := "dagIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	runIdPattern := "runIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``run_id_prefix_pattern`` parameter when possible. (optional)
	runIdPrefixPattern := "runIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	state := []string{"Inner_example"} // []string |  (optional)
	pool := []string{"Inner_example"} // []string |  (optional)
	poolNamePattern := "poolNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``pool_name_prefix_pattern`` parameter when possible. (optional)
	poolNamePrefixPattern := "poolNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	queue := []string{"Inner_example"} // []string |  (optional)
	queueNamePattern := "queueNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``queue_name_prefix_pattern`` parameter when possible. (optional)
	queueNamePrefixPattern := "queueNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	executor := []string{"Inner_example"} // []string |  (optional)
	versionNumber := []int32{int32(123)} // []int32 |  (optional)
	tryNumber := []int32{int32(123)} // []int32 |  (optional)
	operator := []string{"Inner_example"} // []string |  (optional)
	operatorNamePattern := "operatorNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``operator_name_prefix_pattern`` parameter when possible. (optional)
	operatorNamePrefixPattern := "operatorNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	mapIndex := []int32{int32(123)} // []int32 |  (optional)
	renderedMapIndexPattern := "renderedMapIndexPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``rendered_map_index_prefix_pattern`` parameter when possible. (optional)
	renderedMapIndexPrefixPattern := "renderedMapIndexPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	orderBy := []string{"Inner_example"} // []string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `id, state, duration, start_date, end_date, map_index, try_number, logical_date, run_after, data_interval_start, data_interval_end, rendered_map_index, operator, logical_date, run_after, data_interval_start, data_interval_end` (optional) (default to {"map_index"})

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetTaskInstances(context.Background(), dagId, dagRunId).Cursor(cursor).TaskId(taskId).RunAfterGte(runAfterGte).RunAfterGt(runAfterGt).RunAfterLte(runAfterLte).RunAfterLt(runAfterLt).LogicalDateGte(logicalDateGte).LogicalDateGt(logicalDateGt).LogicalDateLte(logicalDateLte).LogicalDateLt(logicalDateLt).StartDateGte(startDateGte).StartDateGt(startDateGt).StartDateLte(startDateLte).StartDateLt(startDateLt).EndDateGte(endDateGte).EndDateGt(endDateGt).EndDateLte(endDateLte).EndDateLt(endDateLt).UpdatedAtGte(updatedAtGte).UpdatedAtGt(updatedAtGt).UpdatedAtLte(updatedAtLte).UpdatedAtLt(updatedAtLt).DurationGte(durationGte).DurationGt(durationGt).DurationLte(durationLte).DurationLt(durationLt).TaskDisplayNamePattern(taskDisplayNamePattern).TaskDisplayNamePrefixPattern(taskDisplayNamePrefixPattern).TaskGroupId(taskGroupId).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).RunIdPattern(runIdPattern).RunIdPrefixPattern(runIdPrefixPattern).State(state).Pool(pool).PoolNamePattern(poolNamePattern).PoolNamePrefixPattern(poolNamePrefixPattern).Queue(queue).QueueNamePattern(queueNamePattern).QueueNamePrefixPattern(queueNamePrefixPattern).Executor(executor).VersionNumber(versionNumber).TryNumber(tryNumber).Operator(operator).OperatorNamePattern(operatorNamePattern).OperatorNamePrefixPattern(operatorNamePrefixPattern).MapIndex(mapIndex).RenderedMapIndexPattern(renderedMapIndexPattern).RenderedMapIndexPrefixPattern(renderedMapIndexPrefixPattern).Limit(limit).Offset(offset).OrderBy(orderBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetTaskInstances``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTaskInstances`: TaskInstanceCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetTaskInstances`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaskInstancesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **cursor** | **string** | Cursor for keyset-based pagination. Pass an empty string for the first page, then use &#x60;&#x60;next_cursor&#x60;&#x60; from the response. When &#x60;&#x60;cursor&#x60;&#x60; is provided, &#x60;&#x60;offset&#x60;&#x60; is ignored. | 
 **taskId** | **string** |  | 
 **runAfterGte** | **time.Time** |  | 
 **runAfterGt** | **time.Time** |  | 
 **runAfterLte** | **time.Time** |  | 
 **runAfterLt** | **time.Time** |  | 
 **logicalDateGte** | **time.Time** |  | 
 **logicalDateGt** | **time.Time** |  | 
 **logicalDateLte** | **time.Time** |  | 
 **logicalDateLt** | **time.Time** |  | 
 **startDateGte** | **time.Time** |  | 
 **startDateGt** | **time.Time** |  | 
 **startDateLte** | **time.Time** |  | 
 **startDateLt** | **time.Time** |  | 
 **endDateGte** | **time.Time** |  | 
 **endDateGt** | **time.Time** |  | 
 **endDateLte** | **time.Time** |  | 
 **endDateLt** | **time.Time** |  | 
 **updatedAtGte** | **time.Time** |  | 
 **updatedAtGt** | **time.Time** |  | 
 **updatedAtLte** | **time.Time** |  | 
 **updatedAtLt** | **time.Time** |  | 
 **durationGte** | **float32** |  | 
 **durationGt** | **float32** |  | 
 **durationLte** | **float32** |  | 
 **durationLt** | **float32** |  | 
 **taskDisplayNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;task_display_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **taskDisplayNamePrefixPattern** | **string** | Prefix match on task display name: optional &#x60;&#x60;_task_display_property_value&#x60;&#x60; else &#x60;&#x60;task_id&#x60;&#x60; (same as &#x60;&#x60;coalesce&#x60;&#x60;). Case-sensitive. Index-friendly alternative to &#x60;&#x60;task_display_name_pattern&#x60;&#x60;. On large databases, combine with &#x60;&#x60;dag_id_prefix_pattern&#x60;&#x60; (or a specific Dag in the path) so &#x60;&#x60;(dag_id, task_id, ...)&#x60;&#x60; indexes apply. Use &#x60;&#x60;|&#x60;&#x60; for OR. Use &#x60;&#x60;~&#x60;&#x60; to match all. Trailing non-alphanumeric characters in the term are stripped before matching so the range scan stays index-compatible under locale-aware collations. | 
 **taskGroupId** | **string** | Filter by exact task group ID. Returns all tasks within the specified task group. | 
 **dagIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;dag_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **dagIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **runIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;run_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **runIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **state** | **[]string** |  | 
 **pool** | **[]string** |  | 
 **poolNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;pool_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **poolNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **queue** | **[]string** |  | 
 **queueNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;queue_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **queueNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **executor** | **[]string** |  | 
 **versionNumber** | **[]int32** |  | 
 **tryNumber** | **[]int32** |  | 
 **operator** | **[]string** |  | 
 **operatorNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;operator_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **operatorNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **mapIndex** | **[]int32** |  | 
 **renderedMapIndexPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;rendered_map_index_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **renderedMapIndexPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;id, state, duration, start_date, end_date, map_index, try_number, logical_date, run_after, data_interval_start, data_interval_end, rendered_map_index, operator, logical_date, run_after, data_interval_start, data_interval_end&#x60; | [default to {&quot;map_index&quot;}]

### Return type

[**TaskInstanceCollectionResponse**](TaskInstanceCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTaskInstancesBatch

> TaskInstanceCollectionResponse GetTaskInstancesBatch(ctx, dagId, dagRunId).TaskInstancesBatchBody(taskInstancesBatchBody).Execute()

Get Task Instances Batch



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskInstancesBatchBody := *openapiclient.NewTaskInstancesBatchBody() // TaskInstancesBatchBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.GetTaskInstancesBatch(context.Background(), dagId, dagRunId).TaskInstancesBatchBody(taskInstancesBatchBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.GetTaskInstancesBatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTaskInstancesBatch`: TaskInstanceCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.GetTaskInstancesBatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTaskInstancesBatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **taskInstancesBatchBody** | [**TaskInstancesBatchBody**](TaskInstancesBatchBody.md) |  | 

### Return type

[**TaskInstanceCollectionResponse**](TaskInstanceCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchTaskInstance

> TaskInstanceCollectionResponse PatchTaskInstance(ctx, dagId, dagRunId, taskId).PatchTaskInstanceBody(patchTaskInstanceBody).MapIndex(mapIndex).UpdateMask(updateMask).Execute()

Patch Task Instance



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	patchTaskInstanceBody := *openapiclient.NewPatchTaskInstanceBody() // PatchTaskInstanceBody | 
	mapIndex := int32(56) // int32 |  (optional)
	updateMask := []string{"Inner_example"} // []string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.PatchTaskInstance(context.Background(), dagId, dagRunId, taskId).PatchTaskInstanceBody(patchTaskInstanceBody).MapIndex(mapIndex).UpdateMask(updateMask).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.PatchTaskInstance``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchTaskInstance`: TaskInstanceCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.PatchTaskInstance`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchTaskInstanceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **patchTaskInstanceBody** | [**PatchTaskInstanceBody**](PatchTaskInstanceBody.md) |  | 
 **mapIndex** | **int32** |  | 
 **updateMask** | **[]string** |  | 

### Return type

[**TaskInstanceCollectionResponse**](TaskInstanceCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchTaskInstanceByMapIndex

> TaskInstanceCollectionResponse PatchTaskInstanceByMapIndex(ctx, dagId, dagRunId, taskId, mapIndex).PatchTaskInstanceBody(patchTaskInstanceBody).UpdateMask(updateMask).Execute()

Patch Task Instance



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 | 
	patchTaskInstanceBody := *openapiclient.NewPatchTaskInstanceBody() // PatchTaskInstanceBody | 
	updateMask := []string{"Inner_example"} // []string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.PatchTaskInstanceByMapIndex(context.Background(), dagId, dagRunId, taskId, mapIndex).PatchTaskInstanceBody(patchTaskInstanceBody).UpdateMask(updateMask).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.PatchTaskInstanceByMapIndex``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchTaskInstanceByMapIndex`: TaskInstanceCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.PatchTaskInstanceByMapIndex`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**mapIndex** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchTaskInstanceByMapIndexRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **patchTaskInstanceBody** | [**PatchTaskInstanceBody**](PatchTaskInstanceBody.md) |  | 
 **updateMask** | **[]string** |  | 

### Return type

[**TaskInstanceCollectionResponse**](TaskInstanceCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchTaskInstanceDryRun

> TaskInstanceCollectionResponse PatchTaskInstanceDryRun(ctx, dagId, dagRunId, taskId).PatchTaskInstanceBody(patchTaskInstanceBody).MapIndex(mapIndex).UpdateMask(updateMask).Execute()

Patch Task Instance Dry Run



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	patchTaskInstanceBody := *openapiclient.NewPatchTaskInstanceBody() // PatchTaskInstanceBody | 
	mapIndex := int32(56) // int32 |  (optional)
	updateMask := []string{"Inner_example"} // []string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.PatchTaskInstanceDryRun(context.Background(), dagId, dagRunId, taskId).PatchTaskInstanceBody(patchTaskInstanceBody).MapIndex(mapIndex).UpdateMask(updateMask).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.PatchTaskInstanceDryRun``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchTaskInstanceDryRun`: TaskInstanceCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.PatchTaskInstanceDryRun`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchTaskInstanceDryRunRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **patchTaskInstanceBody** | [**PatchTaskInstanceBody**](PatchTaskInstanceBody.md) |  | 
 **mapIndex** | **int32** |  | 
 **updateMask** | **[]string** |  | 

### Return type

[**TaskInstanceCollectionResponse**](TaskInstanceCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchTaskInstanceDryRunByMapIndex

> TaskInstanceCollectionResponse PatchTaskInstanceDryRunByMapIndex(ctx, dagId, dagRunId, taskId, mapIndex).PatchTaskInstanceBody(patchTaskInstanceBody).UpdateMask(updateMask).Execute()

Patch Task Instance Dry Run



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 | 
	patchTaskInstanceBody := *openapiclient.NewPatchTaskInstanceBody() // PatchTaskInstanceBody | 
	updateMask := []string{"Inner_example"} // []string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.PatchTaskInstanceDryRunByMapIndex(context.Background(), dagId, dagRunId, taskId, mapIndex).PatchTaskInstanceBody(patchTaskInstanceBody).UpdateMask(updateMask).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.PatchTaskInstanceDryRunByMapIndex``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchTaskInstanceDryRunByMapIndex`: TaskInstanceCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.PatchTaskInstanceDryRunByMapIndex`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**mapIndex** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchTaskInstanceDryRunByMapIndexRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **patchTaskInstanceBody** | [**PatchTaskInstanceBody**](PatchTaskInstanceBody.md) |  | 
 **updateMask** | **[]string** |  | 

### Return type

[**TaskInstanceCollectionResponse**](TaskInstanceCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PostClearTaskInstances

> TaskInstanceCollectionResponse PostClearTaskInstances(ctx, dagId).ClearTaskInstancesBody(clearTaskInstancesBody).Execute()

Post Clear Task Instances



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	clearTaskInstancesBody := *openapiclient.NewClearTaskInstancesBody() // ClearTaskInstancesBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.PostClearTaskInstances(context.Background(), dagId).ClearTaskInstancesBody(clearTaskInstancesBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.PostClearTaskInstances``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PostClearTaskInstances`: TaskInstanceCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.PostClearTaskInstances`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPostClearTaskInstancesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **clearTaskInstancesBody** | [**ClearTaskInstancesBody**](ClearTaskInstancesBody.md) |  | 

### Return type

[**TaskInstanceCollectionResponse**](TaskInstanceCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateHitlDetail

> HITLDetailResponse UpdateHitlDetail(ctx, dagId, dagRunId, taskId, mapIndex).UpdateHITLDetailPayload(updateHITLDetailPayload).Execute()

Update Hitl Detail



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/leonkiss2912/airflow3-client-go"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	taskId := "taskId_example" // string | 
	mapIndex := int32(56) // int32 | 
	updateHITLDetailPayload := *openapiclient.NewUpdateHITLDetailPayload([]string{"ChosenOptions_example"}) // UpdateHITLDetailPayload | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TaskInstanceAPI.UpdateHitlDetail(context.Background(), dagId, dagRunId, taskId, mapIndex).UpdateHITLDetailPayload(updateHITLDetailPayload).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TaskInstanceAPI.UpdateHitlDetail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateHitlDetail`: HITLDetailResponse
	fmt.Fprintf(os.Stdout, "Response from `TaskInstanceAPI.UpdateHitlDetail`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 
**taskId** | **string** |  | 
**mapIndex** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateHitlDetailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **updateHITLDetailPayload** | [**UpdateHITLDetailPayload**](UpdateHITLDetailPayload.md) |  | 

### Return type

[**HITLDetailResponse**](HITLDetailResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

