# \DAGAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteDag**](DAGAPI.md#DeleteDag) | **Delete** /api/v2/dags/{dag_id} | Delete Dag
[**FavoriteDag**](DAGAPI.md#FavoriteDag) | **Post** /api/v2/dags/{dag_id}/favorite | Favorite Dag
[**GetDag**](DAGAPI.md#GetDag) | **Get** /api/v2/dags/{dag_id} | Get Dag
[**GetDagDetails**](DAGAPI.md#GetDagDetails) | **Get** /api/v2/dags/{dag_id}/details | Get Dag Details
[**GetDagTags**](DAGAPI.md#GetDagTags) | **Get** /api/v2/dagTags | Get Dag Tags
[**GetDags**](DAGAPI.md#GetDags) | **Get** /api/v2/dags | Get Dags
[**PatchDag**](DAGAPI.md#PatchDag) | **Patch** /api/v2/dags/{dag_id} | Patch Dag
[**PatchDags**](DAGAPI.md#PatchDags) | **Patch** /api/v2/dags | Patch Dags
[**UnfavoriteDag**](DAGAPI.md#UnfavoriteDag) | **Post** /api/v2/dags/{dag_id}/unfavorite | Unfavorite Dag



## DeleteDag

> interface{} DeleteDag(ctx, dagId).Execute()

Delete Dag



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DAGAPI.DeleteDag(context.Background(), dagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DAGAPI.DeleteDag``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteDag`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `DAGAPI.DeleteDag`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDagRequest struct via the builder pattern


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


## FavoriteDag

> FavoriteDag(ctx, dagId).Execute()

Favorite Dag



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DAGAPI.FavoriteDag(context.Background(), dagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DAGAPI.FavoriteDag``: %v\n", err)
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

Other parameters are passed through a pointer to a apiFavoriteDagRequest struct via the builder pattern


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


## GetDag

> DAGResponse GetDag(ctx, dagId).Execute()

Get Dag



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DAGAPI.GetDag(context.Background(), dagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DAGAPI.GetDag``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDag`: DAGResponse
	fmt.Fprintf(os.Stdout, "Response from `DAGAPI.GetDag`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDagRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DAGResponse**](DAGResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDagDetails

> DAGDetailsResponse GetDagDetails(ctx, dagId).Execute()

Get Dag Details



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DAGAPI.GetDagDetails(context.Background(), dagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DAGAPI.GetDagDetails``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDagDetails`: DAGDetailsResponse
	fmt.Fprintf(os.Stdout, "Response from `DAGAPI.GetDagDetails`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDagDetailsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DAGDetailsResponse**](DAGDetailsResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDagTags

> DAGTagCollectionResponse GetDagTags(ctx).Limit(limit).Offset(offset).OrderBy(orderBy).TagNamePattern(tagNamePattern).TagNamePrefixPattern(tagNamePrefixPattern).Execute()

Get Dag Tags



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
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	orderBy := []string{"Inner_example"} // []string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `name` (optional) (default to {"name"})
	tagNamePattern := "tagNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``tag_name_prefix_pattern`` parameter when possible. (optional)
	tagNamePrefixPattern := "tagNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DAGAPI.GetDagTags(context.Background()).Limit(limit).Offset(offset).OrderBy(orderBy).TagNamePattern(tagNamePattern).TagNamePrefixPattern(tagNamePrefixPattern).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DAGAPI.GetDagTags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDagTags`: DAGTagCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `DAGAPI.GetDagTags`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetDagTagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;name&#x60; | [default to {&quot;name&quot;}]
 **tagNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;tag_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **tagNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 

### Return type

[**DAGTagCollectionResponse**](DAGTagCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDags

> DAGCollectionResponse GetDags(ctx).Limit(limit).Offset(offset).Tags(tags).TagsMatchMode(tagsMatchMode).Owners(owners).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).DagDisplayNamePattern(dagDisplayNamePattern).DagDisplayNamePrefixPattern(dagDisplayNamePrefixPattern).ExcludeStale(excludeStale).Paused(paused).HasImportErrors(hasImportErrors).LastDagRunState(lastDagRunState).BundleName(bundleName).BundleVersion(bundleVersion).HasAssetSchedule(hasAssetSchedule).AssetDependency(assetDependency).DagRunStartDateGte(dagRunStartDateGte).DagRunStartDateGt(dagRunStartDateGt).DagRunStartDateLte(dagRunStartDateLte).DagRunStartDateLt(dagRunStartDateLt).DagRunEndDateGte(dagRunEndDateGte).DagRunEndDateGt(dagRunEndDateGt).DagRunEndDateLte(dagRunEndDateLte).DagRunEndDateLt(dagRunEndDateLt).DagRunState(dagRunState).OrderBy(orderBy).IsFavorite(isFavorite).TimetableType(timetableType).Execute()

Get Dags



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
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	tags := []string{"Inner_example"} // []string |  (optional)
	tagsMatchMode := "tagsMatchMode_example" // string |  (optional)
	owners := []string{"Inner_example"} // []string |  (optional)
	dagIdPattern := "dagIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``dag_id_prefix_pattern`` parameter when possible. (optional)
	dagIdPrefixPattern := "dagIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	dagDisplayNamePattern := "dagDisplayNamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``dag_display_name_prefix_pattern`` parameter when possible. (optional)
	dagDisplayNamePrefixPattern := "dagDisplayNamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	excludeStale := true // bool |  (optional) (default to true)
	paused := true // bool |  (optional)
	hasImportErrors := true // bool | Filter Dags by having import errors. Only Dags that have been successfully loaded before will be returned. (optional)
	lastDagRunState := openapiclient.DagRunState("queued") // DagRunState |  (optional)
	bundleName := "bundleName_example" // string |  (optional)
	bundleVersion := "bundleVersion_example" // string |  (optional)
	hasAssetSchedule := true // bool | Filter Dags with asset-based scheduling (optional)
	assetDependency := "assetDependency_example" // string | Filter Dags by asset dependency (name or URI) (optional)
	dagRunStartDateGte := time.Now() // time.Time |  (optional)
	dagRunStartDateGt := time.Now() // time.Time |  (optional)
	dagRunStartDateLte := time.Now() // time.Time |  (optional)
	dagRunStartDateLt := time.Now() // time.Time |  (optional)
	dagRunEndDateGte := time.Now() // time.Time |  (optional)
	dagRunEndDateGt := time.Now() // time.Time |  (optional)
	dagRunEndDateLte := time.Now() // time.Time |  (optional)
	dagRunEndDateLt := time.Now() // time.Time |  (optional)
	dagRunState := []string{"Inner_example"} // []string |  (optional)
	orderBy := []string{"Inner_example"} // []string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `dag_id, dag_display_name, next_dagrun, state, start_date, last_run_state, last_run_start_date` (optional) (default to {"dag_id"})
	isFavorite := true // bool |  (optional)
	timetableType := []string{"Inner_example"} // []string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DAGAPI.GetDags(context.Background()).Limit(limit).Offset(offset).Tags(tags).TagsMatchMode(tagsMatchMode).Owners(owners).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).DagDisplayNamePattern(dagDisplayNamePattern).DagDisplayNamePrefixPattern(dagDisplayNamePrefixPattern).ExcludeStale(excludeStale).Paused(paused).HasImportErrors(hasImportErrors).LastDagRunState(lastDagRunState).BundleName(bundleName).BundleVersion(bundleVersion).HasAssetSchedule(hasAssetSchedule).AssetDependency(assetDependency).DagRunStartDateGte(dagRunStartDateGte).DagRunStartDateGt(dagRunStartDateGt).DagRunStartDateLte(dagRunStartDateLte).DagRunStartDateLt(dagRunStartDateLt).DagRunEndDateGte(dagRunEndDateGte).DagRunEndDateGt(dagRunEndDateGt).DagRunEndDateLte(dagRunEndDateLte).DagRunEndDateLt(dagRunEndDateLt).DagRunState(dagRunState).OrderBy(orderBy).IsFavorite(isFavorite).TimetableType(timetableType).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DAGAPI.GetDags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDags`: DAGCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `DAGAPI.GetDags`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetDagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **tags** | **[]string** |  | 
 **tagsMatchMode** | **string** |  | 
 **owners** | **[]string** |  | 
 **dagIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;dag_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **dagIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **dagDisplayNamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;dag_display_name_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **dagDisplayNamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **excludeStale** | **bool** |  | [default to true]
 **paused** | **bool** |  | 
 **hasImportErrors** | **bool** | Filter Dags by having import errors. Only Dags that have been successfully loaded before will be returned. | 
 **lastDagRunState** | [**DagRunState**](DagRunState.md) |  | 
 **bundleName** | **string** |  | 
 **bundleVersion** | **string** |  | 
 **hasAssetSchedule** | **bool** | Filter Dags with asset-based scheduling | 
 **assetDependency** | **string** | Filter Dags by asset dependency (name or URI) | 
 **dagRunStartDateGte** | **time.Time** |  | 
 **dagRunStartDateGt** | **time.Time** |  | 
 **dagRunStartDateLte** | **time.Time** |  | 
 **dagRunStartDateLt** | **time.Time** |  | 
 **dagRunEndDateGte** | **time.Time** |  | 
 **dagRunEndDateGt** | **time.Time** |  | 
 **dagRunEndDateLte** | **time.Time** |  | 
 **dagRunEndDateLt** | **time.Time** |  | 
 **dagRunState** | **[]string** |  | 
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;dag_id, dag_display_name, next_dagrun, state, start_date, last_run_state, last_run_start_date&#x60; | [default to {&quot;dag_id&quot;}]
 **isFavorite** | **bool** |  | 
 **timetableType** | **[]string** |  | 

### Return type

[**DAGCollectionResponse**](DAGCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchDag

> DAGResponse PatchDag(ctx, dagId).DAGPatchBody(dAGPatchBody).UpdateMask(updateMask).Execute()

Patch Dag



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
	dAGPatchBody := *openapiclient.NewDAGPatchBody(false) // DAGPatchBody | 
	updateMask := []string{"Inner_example"} // []string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DAGAPI.PatchDag(context.Background(), dagId).DAGPatchBody(dAGPatchBody).UpdateMask(updateMask).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DAGAPI.PatchDag``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchDag`: DAGResponse
	fmt.Fprintf(os.Stdout, "Response from `DAGAPI.PatchDag`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dagId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchDagRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **dAGPatchBody** | [**DAGPatchBody**](DAGPatchBody.md) |  | 
 **updateMask** | **[]string** |  | 

### Return type

[**DAGResponse**](DAGResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PatchDags

> DAGCollectionResponse PatchDags(ctx).DAGPatchBody(dAGPatchBody).UpdateMask(updateMask).Limit(limit).Offset(offset).Tags(tags).TagsMatchMode(tagsMatchMode).Owners(owners).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).ExcludeStale(excludeStale).Paused(paused).Execute()

Patch Dags



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
	dAGPatchBody := *openapiclient.NewDAGPatchBody(false) // DAGPatchBody | 
	updateMask := []string{"Inner_example"} // []string |  (optional)
	limit := int32(56) // int32 |  (optional) (default to 50)
	offset := int32(56) // int32 |  (optional) (default to 0)
	tags := []string{"Inner_example"} // []string |  (optional)
	tagsMatchMode := "tagsMatchMode_example" // string |  (optional)
	owners := []string{"Inner_example"} // []string |  (optional)
	dagIdPattern := "dagIdPattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``dag_id_prefix_pattern`` parameter when possible. (optional)
	dagIdPrefixPattern := "dagIdPrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)
	excludeStale := true // bool |  (optional) (default to true)
	paused := true // bool |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DAGAPI.PatchDags(context.Background()).DAGPatchBody(dAGPatchBody).UpdateMask(updateMask).Limit(limit).Offset(offset).Tags(tags).TagsMatchMode(tagsMatchMode).Owners(owners).DagIdPattern(dagIdPattern).DagIdPrefixPattern(dagIdPrefixPattern).ExcludeStale(excludeStale).Paused(paused).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DAGAPI.PatchDags``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PatchDags`: DAGCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `DAGAPI.PatchDags`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPatchDagsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dAGPatchBody** | [**DAGPatchBody**](DAGPatchBody.md) |  | 
 **updateMask** | **[]string** |  | 
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **tags** | **[]string** |  | 
 **tagsMatchMode** | **string** |  | 
 **owners** | **[]string** |  | 
 **dagIdPattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;dag_id_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **dagIdPrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 
 **excludeStale** | **bool** |  | [default to true]
 **paused** | **bool** |  | 

### Return type

[**DAGCollectionResponse**](DAGCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UnfavoriteDag

> UnfavoriteDag(ctx, dagId).Execute()

Unfavorite Dag



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DAGAPI.UnfavoriteDag(context.Background(), dagId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DAGAPI.UnfavoriteDag``: %v\n", err)
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

Other parameters are passed through a pointer to a apiUnfavoriteDagRequest struct via the builder pattern


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

