# \DagRunAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ClearDagRun**](DagRunAPI.md#ClearDagRun) | **Post** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/clear | Clear Dag Run
[**DeleteDagRun**](DagRunAPI.md#DeleteDagRun) | **Delete** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id} | Delete Dag Run
[**GetDagRun**](DagRunAPI.md#GetDagRun) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id} | Get Dag Run
[**GetDagRuns**](DagRunAPI.md#GetDagRuns) | **Get** /api/v2/dags/{dag_id}/dagRuns | Get Dag Runs
[**GetListDagRunsBatch**](DagRunAPI.md#GetListDagRunsBatch) | **Post** /api/v2/dags/{dag_id}/dagRuns/list | Get List Dag Runs Batch
[**GetUpstreamAssetEvents**](DagRunAPI.md#GetUpstreamAssetEvents) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/upstreamAssetEvents | Get Upstream Asset Events
[**PatchDagRun**](DagRunAPI.md#PatchDagRun) | **Patch** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id} | Patch Dag Run
[**TriggerDagRun**](DagRunAPI.md#TriggerDagRun) | **Post** /api/v2/dags/{dag_id}/dagRuns | Trigger Dag Run
[**WaitDagRunUntilFinished**](DagRunAPI.md#WaitDagRunUntilFinished) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/wait | Experimental: Wait for a dag run to complete, and return task results if requested.



## ClearDagRun

> ResponseClearDagRun ClearDagRun(ctx, dagId, dagRunId).DAGRunClearBody(dAGRunClearBody).Execute()

Clear Dag Run

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
	dAGRunClearBody := *openapiclient.NewDAGRunClearBody() // DAGRunClearBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DagRunAPI.ClearDagRun(context.Background(), dagId, dagRunId).DAGRunClearBody(dAGRunClearBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DagRunAPI.ClearDagRun``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ClearDagRun`: ResponseClearDagRun
	fmt.Fprintf(os.Stdout, "Response from `DagRunAPI.ClearDagRun`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiClearDagRunRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dAGRunClearBody** | [**DAGRunClearBody**](DAGRunClearBody.md) |  | 

### Return type

[**ResponseClearDagRun**](ResponseClearDagRun.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteDagRun

> DeleteDagRun(ctx, dagId, dagRunId).Execute()

Delete Dag Run



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DagRunAPI.DeleteDagRun(context.Background(), dagId, dagRunId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DagRunAPI.DeleteDagRun``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDagRunRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDagRun

> DAGRunResponse GetDagRun(ctx, dagId, dagRunId).Execute()

Get Dag Run

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DagRunAPI.GetDagRun(context.Background(), dagId, dagRunId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DagRunAPI.GetDagRun``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDagRun`: DAGRunResponse
	fmt.Fprintf(os.Stdout, "Response from `DagRunAPI.GetDagRun`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDagRunRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**DAGRunResponse**](DAGRunResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDagRuns

> DAGRunCollectionResponse GetDagRuns(ctx, dagId).Cursor(cursor).Limit(limit).Offset(offset).RunAfterGte(runAfterGte).RunAfterGt(runAfterGt).RunAfterLte(runAfterLte).RunAfterLt(runAfterLt).LogicalDateGte(logicalDateGte).LogicalDateGt(logicalDateGt).LogicalDateLte(logicalDateLte).LogicalDateLt(logicalDateLt).StartDateGte(startDateGte).StartDateGt(startDateGt).StartDateLte(startDateLte).StartDateLt(startDateLt).EndDateGte(endDateGte).EndDateGt(endDateGt).EndDateLte(endDateLte).EndDateLt(endDateLt).DurationGte(durationGte).DurationGt(durationGt).DurationLte(durationLte).DurationLt(durationLt).UpdatedAtGte(updatedAtGte).UpdatedAtGt(updatedAtGt).UpdatedAtLte(updatedAtLte).UpdatedAtLt(updatedAtLt).ConfContains(confContains).RunType(runType).State(state).DagVersion(dagVersion).BundleVersion(bundleVersion).OrderBy(orderBy).RunIdPattern(runIdPattern).RunIdPrefixPattern(runIdPrefixPattern).TriggeringUserNamePattern(triggeringUserNamePattern).TriggeringUserNamePrefixPattern(triggeringUserNamePrefixPattern).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).PartitionKeyPattern(partitionKeyPattern).PartitionKeyPrefixPattern(partitionKeyPrefixPattern).ConsumingAssetPattern(consumingAssetPattern).Execute()

Get Dag Runs



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
	cursor := "cursor_example" // string | Cursor for keyset-based pagination. Pass an empty string for the first page, then use ``next_cursor`` from the response. When ``cursor`` is provided, ``offset`` is ignored. (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
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
	durationGte := float32(8.14) // float32 |  (optional)
	durationGt := float32(8.14) // float32 |  (optional)
	durationLte := float32(8.14) // float32 |  (optional)
	durationLt := float32(8.14) // float32 |  (optional)
	updatedAtGte := time.Now() // time.Time |  (optional)
	updatedAtGt := time.Now() // time.Time |  (optional)
	updatedAtLte := time.Now() // time.Time |  (optional)
	updatedAtLt := time.Now() // time.Time |  (optional)
	confContains := "confContains_example" // string |  (optional)
	runType := []string{"Inner_example"} // []string |  (optional)
	state := []string{"Inner_example"} // []string |  (optional)
	dagVersion := []int32{int32(123)} // []int32 |  (optional)
	bundleVersion := "bundleVersion_example" // string |  (optional)
	orderBy := []string{"Inner_example"} // []string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `id, state, dag_id, run_id, logical_date, run_after, start_date, end_date, updated_at, conf, duration, dag_run_id` (optional) (default to {"id"})
	runIdPattern := "runIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``run_id_prefix_pattern`` parameter when possible. (optional)
	runIdPrefixPattern := "runIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	triggeringUserNamePattern := "triggeringUserNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``triggering_user_name_prefix_pattern`` parameter when possible. (optional)
	triggeringUserNamePrefixPattern := "triggeringUserNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	dagIdPattern := "dagIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``dag_id_prefix_pattern`` parameter when possible. (optional)
	dagIdPrefixPattern := "dagIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	partitionKeyPattern := "partitionKeyPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``partition_key_prefix_pattern`` parameter when possible. (optional)
	partitionKeyPrefixPattern := "partitionKeyPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	consumingAssetPattern := "consumingAssetPattern_example" // string | Filter by consuming asset name or URI using pattern matching (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DagRunAPI.GetDagRuns(context.Background(), dagId).Cursor(cursor).Limit(limit).Offset(offset).RunAfterGte(runAfterGte).RunAfterGt(runAfterGt).RunAfterLte(runAfterLte).RunAfterLt(runAfterLt).LogicalDateGte(logicalDateGte).LogicalDateGt(logicalDateGt).LogicalDateLte(logicalDateLte).LogicalDateLt(logicalDateLt).StartDateGte(startDateGte).StartDateGt(startDateGt).StartDateLte(startDateLte).StartDateLt(startDateLt).EndDateGte(endDateGte).EndDateGt(endDateGt).EndDateLte(endDateLte).EndDateLt(endDateLt).DurationGte(durationGte).DurationGt(durationGt).DurationLte(durationLte).DurationLt(durationLt).UpdatedAtGte(updatedAtGte).UpdatedAtGt(updatedAtGt).UpdatedAtLte(updatedAtLte).UpdatedAtLt(updatedAtLt).ConfContains(confContains).RunType(runType).State(state).DagVersion(dagVersion).BundleVersion(bundleVersion).OrderBy(orderBy).RunIdPattern(runIdPattern).RunIdPrefixPattern(runIdPrefixPattern).TriggeringUserNamePattern(triggeringUserNamePattern).TriggeringUserNamePrefixPattern(triggeringUserNamePrefixPattern).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).PartitionKeyPattern(partitionKeyPattern).PartitionKeyPrefixPattern(partitionKeyPrefixPattern).ConsumingAssetPattern(consumingAssetPattern).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DagRunAPI.GetDagRuns``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDagRuns`: DAGRunCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `DagRunAPI.GetDagRuns`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDagRunsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **cursor** | **string** | Cursor for keyset-based pagination. Pass an empty string for the first page, then use &#x60;&#x60;next_cursor&#x60;&#x60; from the response. When &#x60;&#x60;cursor&#x60;&#x60; is provided, &#x60;&#x60;offset&#x60;&#x60; is ignored. | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
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
 **durationGte** | **float32** |  | 
 **durationGt** | **float32** |  | 
 **durationLte** | **float32** |  | 
 **durationLt** | **float32** |  | 
 **updatedAtGte** | **time.Time** |  | 
 **updatedAtGt** | **time.Time** |  | 
 **updatedAtLte** | **time.Time** |  | 
 **updatedAtLt** | **time.Time** |  | 
 **confContains** | **string** |  | 
 **runType** | **[]string** |  | 
 **state** | **[]string** |  | 
 **dagVersion** | **[]int32** |  | 
 **bundleVersion** | **string** |  | 
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;id, state, dag_id, run_id, logical_date, run_after, start_date, end_date, updated_at, conf, duration, dag_run_id&#x60; | [default to {&quot;id&quot;}]
 **runIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;run_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **runIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **triggeringUserNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;triggering_user_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **triggeringUserNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **dagIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;dag_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **dagIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **partitionKeyPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;partition_key_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **partitionKeyPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **consumingAssetPattern** | **string** | Filter by consuming asset name or URI using pattern matching | 

### Return type

[**DAGRunCollectionResponse**](DAGRunCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetListDagRunsBatch

> DAGRunCollectionResponse GetListDagRunsBatch(ctx, dagId).DAGRunsBatchBody(dAGRunsBatchBody).Execute()

Get List Dag Runs Batch



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
	dAGRunsBatchBody := *openapiclient.NewDAGRunsBatchBody() // DAGRunsBatchBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DagRunAPI.GetListDagRunsBatch(context.Background(), dagId).DAGRunsBatchBody(dAGRunsBatchBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DagRunAPI.GetListDagRunsBatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetListDagRunsBatch`: DAGRunCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `DagRunAPI.GetListDagRunsBatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetListDagRunsBatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dAGRunsBatchBody** | [**DAGRunsBatchBody**](DAGRunsBatchBody.md) |  | 

### Return type

[**DAGRunCollectionResponse**](DAGRunCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUpstreamAssetEvents

> AssetEventCollectionResponse GetUpstreamAssetEvents(ctx, dagId, dagRunId).Execute()

Get Upstream Asset Events



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DagRunAPI.GetUpstreamAssetEvents(context.Background(), dagId, dagRunId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DagRunAPI.GetUpstreamAssetEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUpstreamAssetEvents`: AssetEventCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `DagRunAPI.GetUpstreamAssetEvents`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetUpstreamAssetEventsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**AssetEventCollectionResponse**](AssetEventCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchDagRun

> DAGRunResponse PatchDagRun(ctx, dagId, dagRunId).DAGRunPatchBody(dAGRunPatchBody).UpdateMask(updateMask).Execute()

Patch Dag Run



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
	dAGRunPatchBody := *openapiclient.NewDAGRunPatchBody() // DAGRunPatchBody | 
	updateMask := []string{"Inner_example"} // []string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DagRunAPI.PatchDagRun(context.Background(), dagId, dagRunId).DAGRunPatchBody(dAGRunPatchBody).UpdateMask(updateMask).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DagRunAPI.PatchDagRun``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchDagRun`: DAGRunResponse
	fmt.Fprintf(os.Stdout, "Response from `DagRunAPI.PatchDagRun`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchDagRunRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **dAGRunPatchBody** | [**DAGRunPatchBody**](DAGRunPatchBody.md) |  | 
 **updateMask** | **[]string** |  | 

### Return type

[**DAGRunResponse**](DAGRunResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TriggerDagRun

> DAGRunResponse TriggerDagRun(ctx, dagId).TriggerDAGRunPostBody(triggerDAGRunPostBody).Execute()

Trigger Dag Run



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
	dagId := TODO // interface{} | 
	triggerDAGRunPostBody := *openapiclient.NewTriggerDAGRunPostBody(time.Now()) // TriggerDAGRunPostBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DagRunAPI.TriggerDagRun(context.Background(), dagId).TriggerDAGRunPostBody(triggerDAGRunPostBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DagRunAPI.TriggerDagRun``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TriggerDagRun`: DAGRunResponse
	fmt.Fprintf(os.Stdout, "Response from `DagRunAPI.TriggerDagRun`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | [**interface{}**](.md) |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTriggerDagRunRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **triggerDAGRunPostBody** | [**TriggerDAGRunPostBody**](TriggerDAGRunPostBody.md) |  | 

### Return type

[**DAGRunResponse**](DAGRunResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WaitDagRunUntilFinished

> interface{} WaitDagRunUntilFinished(ctx, dagId, dagRunId).Interval(interval).Result(result).Execute()

Experimental: Wait for a dag run to complete, and return task results if requested.



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
	interval := float32(8.14) // float32 | Seconds to wait between dag run state checks
	result := []string{"Inner_example"} // []string | Collect result XCom from task. Can be set multiple times. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DagRunAPI.WaitDagRunUntilFinished(context.Background(), dagId, dagRunId).Interval(interval).Result(result).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DagRunAPI.WaitDagRunUntilFinished``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WaitDagRunUntilFinished`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DagRunAPI.WaitDagRunUntilFinished`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiWaitDagRunUntilFinishedRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **interval** | **float32** | Seconds to wait between dag run state checks | 
 **result** | **[]string** | Collect result XCom from task. Can be set multiple times. | 

### Return type

**interface{}**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/x-ndjson

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

