# \XComAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateXcomEntry**](XComAPI.md#CreateXcomEntry) | **Post** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/xcomEntries | Create Xcom Entry
[**DeleteXcomEntry**](XComAPI.md#DeleteXcomEntry) | **Delete** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/xcomEntries/{xcom_key} | Delete Xcom Entry
[**GetXcomEntries**](XComAPI.md#GetXcomEntries) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/xcomEntries | Get Xcom Entries
[**GetXcomEntry**](XComAPI.md#GetXcomEntry) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/xcomEntries/{xcom_key} | Get Xcom Entry
[**UpdateXcomEntry**](XComAPI.md#UpdateXcomEntry) | **Patch** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/taskInstances/{task_id}/xcomEntries/{xcom_key} | Update Xcom Entry



## CreateXcomEntry

> XComResponseNative CreateXcomEntry(ctx, dagId, taskId, dagRunId).XComCreateBody(xComCreateBody).Execute()

Create Xcom Entry



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
	taskId := "taskId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	xComCreateBody := *openapiclient.NewXComCreateBody("Key_example", interface{}(123)) // XComCreateBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.XComAPI.CreateXcomEntry(context.Background(), dagId, taskId, dagRunId).XComCreateBody(xComCreateBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `XComAPI.CreateXcomEntry``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateXcomEntry`: XComResponseNative
	fmt.Fprintf(os.Stdout, "Response from `XComAPI.CreateXcomEntry`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**taskId** | **string** |  | 
**dagRunId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateXcomEntryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **xComCreateBody** | [**XComCreateBody**](XComCreateBody.md) |  | 

### Return type

[**XComResponseNative**](XComResponseNative.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteXcomEntry

> DeleteXcomEntry(ctx, dagId, taskId, dagRunId, xcomKey).MapIndex(mapIndex).Execute()

Delete Xcom Entry



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
	taskId := "taskId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	xcomKey := "xcomKey_example" // string | 
	mapIndex := int32(56) // int32 |  (optional) (default to -1)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.XComAPI.DeleteXcomEntry(context.Background(), dagId, taskId, dagRunId, xcomKey).MapIndex(mapIndex).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `XComAPI.DeleteXcomEntry``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**taskId** | **string** |  | 
**dagRunId** | **string** |  | 
**xcomKey** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteXcomEntryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **mapIndex** | **int32** |  | [default to -1]

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


## GetXcomEntries

> XComCollectionResponse GetXcomEntries(ctx, dagId, dagRunId, taskId).XcomKey(xcomKey).MapIndex(mapIndex).Limit(limit).Offset(offset).XcomKeyPattern(xcomKeyPattern).XcomKeyPrefixPattern(xcomKeyPrefixPattern).DagDisplayNamePattern(dagDisplayNamePattern).DagDisplayNamePrefixPattern(dagDisplayNamePrefixPattern).RunIdPattern(runIdPattern).RunIdPrefixPattern(runIdPrefixPattern).TaskIdPattern(taskIdPattern).TaskIdPrefixPattern(taskIdPrefixPattern).MapIndexFilter(mapIndexFilter).LogicalDateGte(logicalDateGte).LogicalDateGt(logicalDateGt).LogicalDateLte(logicalDateLte).LogicalDateLt(logicalDateLt).RunAfterGte(runAfterGte).RunAfterGt(runAfterGt).RunAfterLte(runAfterLte).RunAfterLt(runAfterLt).OrderBy(orderBy).Execute()

Get Xcom Entries



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
	xcomKey := "xcomKey_example" // string |  (optional)
	mapIndex := int32(56) // int32 |  (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	xcomKeyPattern := "xcomKeyPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``xcom_key_prefix_pattern`` parameter when possible. (optional)
	xcomKeyPrefixPattern := "xcomKeyPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	dagDisplayNamePattern := "dagDisplayNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``dag_display_name_prefix_pattern`` parameter when possible. (optional)
	dagDisplayNamePrefixPattern := "dagDisplayNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	runIdPattern := "runIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``run_id_prefix_pattern`` parameter when possible. (optional)
	runIdPrefixPattern := "runIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	taskIdPattern := "taskIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``task_id_prefix_pattern`` parameter when possible. (optional)
	taskIdPrefixPattern := "taskIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	mapIndexFilter := int32(56) // int32 |  (optional)
	logicalDateGte := time.Now() // time.Time |  (optional)
	logicalDateGt := time.Now() // time.Time |  (optional)
	logicalDateLte := time.Now() // time.Time |  (optional)
	logicalDateLt := time.Now() // time.Time |  (optional)
	runAfterGte := time.Now() // time.Time |  (optional)
	runAfterGt := time.Now() // time.Time |  (optional)
	runAfterLte := time.Now() // time.Time |  (optional)
	runAfterLt := time.Now() // time.Time |  (optional)
	orderBy := []string{"Inner_example"} // []string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `key, dag_id, run_id, task_id, map_index, timestamp, run_after` (optional) (default to {"dag_id", "task_id", "run_id", "map_index", "key"})

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.XComAPI.GetXcomEntries(context.Background(), dagId, dagRunId, taskId).XcomKey(xcomKey).MapIndex(mapIndex).Limit(limit).Offset(offset).XcomKeyPattern(xcomKeyPattern).XcomKeyPrefixPattern(xcomKeyPrefixPattern).DagDisplayNamePattern(dagDisplayNamePattern).DagDisplayNamePrefixPattern(dagDisplayNamePrefixPattern).RunIdPattern(runIdPattern).RunIdPrefixPattern(runIdPrefixPattern).TaskIdPattern(taskIdPattern).TaskIdPrefixPattern(taskIdPrefixPattern).MapIndexFilter(mapIndexFilter).LogicalDateGte(logicalDateGte).LogicalDateGt(logicalDateGt).LogicalDateLte(logicalDateLte).LogicalDateLt(logicalDateLt).RunAfterGte(runAfterGte).RunAfterGt(runAfterGt).RunAfterLte(runAfterLte).RunAfterLt(runAfterLt).OrderBy(orderBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `XComAPI.GetXcomEntries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetXcomEntries`: XComCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `XComAPI.GetXcomEntries`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiGetXcomEntriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **xcomKey** | **string** |  | 
 **mapIndex** | **int32** |  | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **xcomKeyPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;xcom_key_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **xcomKeyPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **dagDisplayNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;dag_display_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **dagDisplayNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **runIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;run_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **runIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **taskIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;task_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **taskIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **mapIndexFilter** | **int32** |  | 
 **logicalDateGte** | **time.Time** |  | 
 **logicalDateGt** | **time.Time** |  | 
 **logicalDateLte** | **time.Time** |  | 
 **logicalDateLt** | **time.Time** |  | 
 **runAfterGte** | **time.Time** |  | 
 **runAfterGt** | **time.Time** |  | 
 **runAfterLte** | **time.Time** |  | 
 **runAfterLt** | **time.Time** |  | 
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;key, dag_id, run_id, task_id, map_index, timestamp, run_after&#x60; | [default to {&quot;dag_id&quot;, &quot;task_id&quot;, &quot;run_id&quot;, &quot;map_index&quot;, &quot;key&quot;}]

### Return type

[**XComCollectionResponse**](XComCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetXcomEntry

> ResponseGetXcomEntry GetXcomEntry(ctx, dagId, taskId, dagRunId, xcomKey).MapIndex(mapIndex).Deserialize(deserialize).Stringify(stringify).Execute()

Get Xcom Entry



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
	taskId := "taskId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	xcomKey := "xcomKey_example" // string | 
	mapIndex := int32(56) // int32 |  (optional) (default to -1)
	deserialize := true // bool |  (optional) (default to false)
	stringify := true // bool |  (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.XComAPI.GetXcomEntry(context.Background(), dagId, taskId, dagRunId, xcomKey).MapIndex(mapIndex).Deserialize(deserialize).Stringify(stringify).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `XComAPI.GetXcomEntry``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetXcomEntry`: ResponseGetXcomEntry
	fmt.Fprintf(os.Stdout, "Response from `XComAPI.GetXcomEntry`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**taskId** | **string** |  | 
**dagRunId** | **string** |  | 
**xcomKey** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetXcomEntryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **mapIndex** | **int32** |  | [default to -1]
 **deserialize** | **bool** |  | [default to false]
 **stringify** | **bool** |  | [default to false]

### Return type

[**ResponseGetXcomEntry**](ResponseGetXcomEntry.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateXcomEntry

> XComResponseNative UpdateXcomEntry(ctx, dagId, taskId, dagRunId, xcomKey).XComUpdateBody(xComUpdateBody).Execute()

Update Xcom Entry



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
	taskId := "taskId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	xcomKey := "xcomKey_example" // string | 
	xComUpdateBody := *openapiclient.NewXComUpdateBody(interface{}(123)) // XComUpdateBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.XComAPI.UpdateXcomEntry(context.Background(), dagId, taskId, dagRunId, xcomKey).XComUpdateBody(xComUpdateBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `XComAPI.UpdateXcomEntry``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateXcomEntry`: XComResponseNative
	fmt.Fprintf(os.Stdout, "Response from `XComAPI.UpdateXcomEntry`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**taskId** | **string** |  | 
**dagRunId** | **string** |  | 
**xcomKey** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateXcomEntryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




 **xComUpdateBody** | [**XComUpdateBody**](XComUpdateBody.md) |  | 

### Return type

[**XComResponseNative**](XComResponseNative.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

