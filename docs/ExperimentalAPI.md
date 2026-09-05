# \ExperimentalAPI

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**WaitDagRunUntilFinished**](ExperimentalAPI.md#WaitDagRunUntilFinished) | **Get** /api/v2/dags/{dag_id}/dagRuns/{dag_run_id}/wait | Experimental: Wait for a dag run to complete, and return task results if requested.



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
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID/airflow"
)

func main() {
	dagId := "dagId_example" // string | 
	dagRunId := "dagRunId_example" // string | 
	interval := float32(8.14) // float32 | Seconds to wait between dag run state checks
	result := []string{"Inner_example"} // []string | Collect result XCom from task. Can be set multiple times. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ExperimentalAPI.WaitDagRunUntilFinished(context.Background(), dagId, dagRunId).Interval(interval).Result(result).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ExperimentalAPI.WaitDagRunUntilFinished``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WaitDagRunUntilFinished`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `ExperimentalAPI.WaitDagRunUntilFinished`: %v\n", resp)
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

