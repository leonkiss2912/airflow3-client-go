# \AssetAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAssetEvent**](AssetAPI.md#CreateAssetEvent) | **Post** /api/v2/assets/events | Create Asset Event
[**DeleteAssetQueuedEvents**](AssetAPI.md#DeleteAssetQueuedEvents) | **Delete** /api/v2/assets/{asset_id}/queuedEvents | Delete Asset Queued Events
[**DeleteDagAssetQueuedEvent**](AssetAPI.md#DeleteDagAssetQueuedEvent) | **Delete** /api/v2/dags/{dag_id}/assets/{asset_id}/queuedEvents | Delete Dag Asset Queued Event
[**DeleteDagAssetQueuedEvents**](AssetAPI.md#DeleteDagAssetQueuedEvents) | **Delete** /api/v2/dags/{dag_id}/assets/queuedEvents | Delete Dag Asset Queued Events
[**GetAsset**](AssetAPI.md#GetAsset) | **Get** /api/v2/assets/{asset_id} | Get Asset
[**GetAssetAlias**](AssetAPI.md#GetAssetAlias) | **Get** /api/v2/assets/aliases/{asset_alias_id} | Get Asset Alias
[**GetAssetAliases**](AssetAPI.md#GetAssetAliases) | **Get** /api/v2/assets/aliases | Get Asset Aliases
[**GetAssetEvents**](AssetAPI.md#GetAssetEvents) | **Get** /api/v2/assets/events | Get Asset Events
[**GetAssetQueuedEvents**](AssetAPI.md#GetAssetQueuedEvents) | **Get** /api/v2/assets/{asset_id}/queuedEvents | Get Asset Queued Events
[**GetAssets**](AssetAPI.md#GetAssets) | **Get** /api/v2/assets | Get Assets
[**GetDagAssetQueuedEvent**](AssetAPI.md#GetDagAssetQueuedEvent) | **Get** /api/v2/dags/{dag_id}/assets/{asset_id}/queuedEvents | Get Dag Asset Queued Event
[**GetDagAssetQueuedEvents**](AssetAPI.md#GetDagAssetQueuedEvents) | **Get** /api/v2/dags/{dag_id}/assets/queuedEvents | Get Dag Asset Queued Events
[**MaterializeAsset**](AssetAPI.md#MaterializeAsset) | **Post** /api/v2/assets/{asset_id}/materialize | Materialize Asset



## CreateAssetEvent

> AssetEventResponse CreateAssetEvent(ctx).CreateAssetEventsBody(createAssetEventsBody).Execute()

Create Asset Event



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	createAssetEventsBody := *openapiclient.NewCreateAssetEventsBody(int32(123)) // CreateAssetEventsBody | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.CreateAssetEvent(context.Background()).CreateAssetEventsBody(createAssetEventsBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.CreateAssetEvent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAssetEvent`: AssetEventResponse
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.CreateAssetEvent`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateAssetEventRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createAssetEventsBody** | [**CreateAssetEventsBody**](CreateAssetEventsBody.md) |  | 

### Return type

[**AssetEventResponse**](AssetEventResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteAssetQueuedEvents

> DeleteAssetQueuedEvents(ctx, assetId).Before(before).Execute()

Delete Asset Queued Events



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	assetId := int32(56) // int32 | 
	before := "before_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AssetAPI.DeleteAssetQueuedEvents(context.Background(), assetId).Before(before).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.DeleteAssetQueuedEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**assetId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAssetQueuedEventsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **before** | **string** |  | 

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


## DeleteDagAssetQueuedEvent

> DeleteDagAssetQueuedEvent(ctx, dagId, assetId).Before(before).Execute()

Delete Dag Asset Queued Event



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	dagId := "dagId_example" // string | 
	assetId := int32(56) // int32 | 
	before := "before_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AssetAPI.DeleteDagAssetQueuedEvent(context.Background(), dagId, assetId).Before(before).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.DeleteDagAssetQueuedEvent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**assetId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDagAssetQueuedEventRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **before** | **string** |  | 

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


## DeleteDagAssetQueuedEvents

> DeleteDagAssetQueuedEvents(ctx, dagId).Before(before).Execute()

Delete Dag Asset Queued Events

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	dagId := "dagId_example" // string | 
	before := "before_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AssetAPI.DeleteDagAssetQueuedEvents(context.Background(), dagId).Before(before).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.DeleteDagAssetQueuedEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDagAssetQueuedEventsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **before** | **string** |  | 

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


## GetAsset

> AssetResponse GetAsset(ctx, assetId).Execute()

Get Asset



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	assetId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.GetAsset(context.Background(), assetId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.GetAsset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAsset`: AssetResponse
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.GetAsset`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**assetId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAssetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**AssetResponse**](AssetResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAssetAlias

> interface{} GetAssetAlias(ctx, assetAliasId).Execute()

Get Asset Alias



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	assetAliasId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.GetAssetAlias(context.Background(), assetAliasId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.GetAssetAlias``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAssetAlias`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.GetAssetAlias`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**assetAliasId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAssetAliasRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


## GetAssetAliases

> AssetAliasCollectionResponse GetAssetAliases(ctx).Limit(limit).Offset(offset).NamePattern(namePattern).NamePrefixPattern(namePrefixPattern).OrderBy(orderBy).Execute()

Get Asset Aliases



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	namePattern := "namePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``name_prefix_pattern`` parameter when possible. (optional)
	namePrefixPattern := "namePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	orderBy := []*string{"Inner_example"} // []*string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `id, name` (optional) (default to {"id"})

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.GetAssetAliases(context.Background()).Limit(limit).Offset(offset).NamePattern(namePattern).NamePrefixPattern(namePrefixPattern).OrderBy(orderBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.GetAssetAliases``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAssetAliases`: AssetAliasCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.GetAssetAliases`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetAssetAliasesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **namePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **namePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;id, name&#x60; | [default to {&quot;id&quot;}]

### Return type

[**AssetAliasCollectionResponse**](AssetAliasCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAssetEvents

> AssetEventCollectionResponse GetAssetEvents(ctx).Limit(limit).Offset(offset).OrderBy(orderBy).AssetId(assetId).SourceDagId(sourceDagId).SourceTaskId(sourceTaskId).SourceRunId(sourceRunId).SourceMapIndex(sourceMapIndex).NamePattern(namePattern).NamePrefixPattern(namePrefixPattern).TimestampGte(timestampGte).TimestampGt(timestampGt).TimestampLte(timestampLte).TimestampLt(timestampLt).Execute()

Get Asset Events



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
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	orderBy := []*string{"Inner_example"} // []*string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `source_task_id, source_dag_id, source_run_id, source_map_index, timestamp` (optional) (default to {"timestamp"})
	assetId := int32(56) // int32 |  (optional)
	sourceDagId := "sourceDagId_example" // string |  (optional)
	sourceTaskId := "sourceTaskId_example" // string |  (optional)
	sourceRunId := "sourceRunId_example" // string |  (optional)
	sourceMapIndex := int32(56) // int32 |  (optional)
	namePattern := "namePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``name_prefix_pattern`` parameter when possible. (optional)
	namePrefixPattern := "namePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	timestampGte := time.Now() // time.Time |  (optional)
	timestampGt := time.Now() // time.Time |  (optional)
	timestampLte := time.Now() // time.Time |  (optional)
	timestampLt := time.Now() // time.Time |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.GetAssetEvents(context.Background()).Limit(limit).Offset(offset).OrderBy(orderBy).AssetId(assetId).SourceDagId(sourceDagId).SourceTaskId(sourceTaskId).SourceRunId(sourceRunId).SourceMapIndex(sourceMapIndex).NamePattern(namePattern).NamePrefixPattern(namePrefixPattern).TimestampGte(timestampGte).TimestampGt(timestampGt).TimestampLte(timestampLte).TimestampLt(timestampLt).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.GetAssetEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAssetEvents`: AssetEventCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.GetAssetEvents`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetAssetEventsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;source_task_id, source_dag_id, source_run_id, source_map_index, timestamp&#x60; | [default to {&quot;timestamp&quot;}]
 **assetId** | **int32** |  | 
 **sourceDagId** | **string** |  | 
 **sourceTaskId** | **string** |  | 
 **sourceRunId** | **string** |  | 
 **sourceMapIndex** | **int32** |  | 
 **namePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **namePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **timestampGte** | **time.Time** |  | 
 **timestampGt** | **time.Time** |  | 
 **timestampLte** | **time.Time** |  | 
 **timestampLt** | **time.Time** |  | 

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


## GetAssetQueuedEvents

> QueuedEventCollectionResponse GetAssetQueuedEvents(ctx, assetId).Before(before).Execute()

Get Asset Queued Events



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	assetId := int32(56) // int32 | 
	before := "before_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.GetAssetQueuedEvents(context.Background(), assetId).Before(before).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.GetAssetQueuedEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAssetQueuedEvents`: QueuedEventCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.GetAssetQueuedEvents`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**assetId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAssetQueuedEventsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **before** | **string** |  | 

### Return type

[**QueuedEventCollectionResponse**](QueuedEventCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAssets

> AssetCollectionResponse GetAssets(ctx).Limit(limit).Offset(offset).NamePattern(namePattern).NamePrefixPattern(namePrefixPattern).UriPattern(uriPattern).UriPrefixPattern(uriPrefixPattern).DagIds(dagIds).OnlyActive(onlyActive).OrderBy(orderBy).Execute()

Get Assets



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	namePattern := "namePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``name_prefix_pattern`` parameter when possible. (optional)
	namePrefixPattern := "namePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	uriPattern := "uriPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``uri_prefix_pattern`` parameter when possible. (optional)
	uriPrefixPattern := "uriPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	dagIds := []*string{"Inner_example"} // []*string |  (optional)
	onlyActive := true // bool |  (optional) (default to true)
	orderBy := []*string{"Inner_example"} // []*string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `id, name, uri, created_at, updated_at` (optional) (default to {"id"})

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.GetAssets(context.Background()).Limit(limit).Offset(offset).NamePattern(namePattern).NamePrefixPattern(namePrefixPattern).UriPattern(uriPattern).UriPrefixPattern(uriPrefixPattern).DagIds(dagIds).OnlyActive(onlyActive).OrderBy(orderBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.GetAssets``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAssets`: AssetCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.GetAssets`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetAssetsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **namePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **namePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **uriPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;uri_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **uriPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **dagIds** | **[]string** |  | 
 **onlyActive** | **bool** |  | [default to true]
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;id, name, uri, created_at, updated_at&#x60; | [default to {&quot;id&quot;}]

### Return type

[**AssetCollectionResponse**](AssetCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDagAssetQueuedEvent

> QueuedEventResponse GetDagAssetQueuedEvent(ctx, dagId, assetId).Before(before).Execute()

Get Dag Asset Queued Event



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	dagId := "dagId_example" // string | 
	assetId := int32(56) // int32 | 
	before := "before_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.GetDagAssetQueuedEvent(context.Background(), dagId, assetId).Before(before).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.GetDagAssetQueuedEvent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDagAssetQueuedEvent`: QueuedEventResponse
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.GetDagAssetQueuedEvent`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 
**assetId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDagAssetQueuedEventRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **before** | **string** |  | 

### Return type

[**QueuedEventResponse**](QueuedEventResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDagAssetQueuedEvents

> QueuedEventCollectionResponse GetDagAssetQueuedEvents(ctx, dagId).Before(before).Execute()

Get Dag Asset Queued Events



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	dagId := "dagId_example" // string | 
	before := "before_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.GetDagAssetQueuedEvents(context.Background(), dagId).Before(before).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.GetDagAssetQueuedEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDagAssetQueuedEvents`: QueuedEventCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.GetDagAssetQueuedEvents`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDagAssetQueuedEventsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **before** | **string** |  | 

### Return type

[**QueuedEventCollectionResponse**](QueuedEventCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## MaterializeAsset

> DAGRunResponse MaterializeAsset(ctx, assetId).MaterializeAssetBody(materializeAssetBody).Execute()

Materialize Asset



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	assetId := int32(56) // int32 | 
	materializeAssetBody := *openapiclient.NewMaterializeAssetBody() // MaterializeAssetBody |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssetAPI.MaterializeAsset(context.Background(), assetId).MaterializeAssetBody(materializeAssetBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssetAPI.MaterializeAsset``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MaterializeAsset`: DAGRunResponse
	fmt.Fprintf(os.Stdout, "Response from `AssetAPI.MaterializeAsset`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**assetId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiMaterializeAssetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **materializeAssetBody** | [**MaterializeAssetBody**](MaterializeAssetBody.md) |  | 

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

