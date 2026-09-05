# \ImportErrorAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetImportError**](ImportErrorAPI.md#GetImportError) | **Get** /api/v2/importErrors/{import_error_id} | Get Import Error
[**GetImportErrors**](ImportErrorAPI.md#GetImportErrors) | **Get** /api/v2/importErrors | Get Import Errors



## GetImportError

> ImportErrorResponse GetImportError(ctx, importErrorId).Execute()

Get Import Error



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
	importErrorId := int32(56) // int32 | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportErrorAPI.GetImportError(context.Background(), importErrorId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportErrorAPI.GetImportError``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetImportError`: ImportErrorResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportErrorAPI.GetImportError`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**importErrorId** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetImportErrorRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ImportErrorResponse**](ImportErrorResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetImportErrors

> ImportErrorCollectionResponse GetImportErrors(ctx).Limit(limit).Offset(offset).OrderBy(orderBy).FilenamePattern(filenamePattern).FilenamePrefixPattern(filenamePrefixPattern).Execute()

Get Import Errors



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
	orderBy := []string{"Inner_example"} // []string | Attributes to order by, multi criteria sort is supported. Prefix with `-` for descending order. Supported attributes: `id, timestamp, filename, bundle_name, stacktrace, import_error_id` (optional) (default to {"id"})
	filenamePattern := "filenamePattern_example" // string | SQL LIKE expression — use `%` / `_` wildcards (e.g. `%customer_%`). or the pipe `|` operator for OR logic (e.g. `dag1 | dag2`). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as ``ILIKE '%term%'`` and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent ``filename_prefix_pattern`` parameter when possible. (optional)
	filenamePrefixPattern := "filenamePrefixPattern_example" // string | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe `|` operator for OR logic (e.g. `dag1|dag2`). Use `~` to match all. Wildcard characters (`%`, `_`) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. `test_` effectively matches items starting with `test`, and `s3://` matches items starting with `s3`. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ImportErrorAPI.GetImportErrors(context.Background()).Limit(limit).Offset(offset).OrderBy(orderBy).FilenamePattern(filenamePattern).FilenamePrefixPattern(filenamePrefixPattern).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ImportErrorAPI.GetImportErrors``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetImportErrors`: ImportErrorCollectionResponse
	fmt.Fprintf(os.Stdout, "Response from `ImportErrorAPI.GetImportErrors`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetImportErrorsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int32** |  | [default to 50]
 **offset** | **int32** |  | [default to 0]
 **orderBy** | **[]string** | Attributes to order by, multi criteria sort is supported. Prefix with &#x60;-&#x60; for descending order. Supported attributes: &#x60;id, timestamp, filename, bundle_name, stacktrace, import_error_id&#x60; | [default to {&quot;id&quot;}]
 **filenamePattern** | **string** | SQL LIKE expression — use &#x60;%&#x60; / &#x60;_&#x60; wildcards (e.g. &#x60;%customer_%&#x60;). or the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1 | dag2&#x60;). Regular expressions are **not** supported.   **Performance note:** this full-match pattern is evaluated as &#x60;&#x60;ILIKE &#39;%term%&#39;&#x60;&#x60; and most of the time prevents the database from using B-tree indexes, which can be very slow on large tables. Prefer the equivalent &#x60;&#x60;filename_prefix_pattern&#x60;&#x60; parameter when possible. | 
 **filenamePrefixPattern** | **string** | Prefix match — returns items whose value starts with the given string (case-sensitive, index-friendly). Use the pipe &#x60;|&#x60; operator for OR logic (e.g. &#x60;dag1|dag2&#x60;). Use &#x60;~&#x60; to match all. Wildcard characters (&#x60;%&#x60;, &#x60;_&#x60;) are treated as literal characters. Trailing non-alphanumeric characters in the prefix are stripped before matching so the range scan stays index-compatible under locale-aware collations — e.g. &#x60;test_&#x60; effectively matches items starting with &#x60;test&#x60;, and &#x60;s3://&#x60; matches items starting with &#x60;s3&#x60;. | 

### Return type

[**ImportErrorCollectionResponse**](ImportErrorCollectionResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer), [HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

