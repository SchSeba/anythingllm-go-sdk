# \UserManagementAPI

All URIs are relative to *https://raw.githubusercontent.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**V1UsersGet**](UserManagementAPI.md#V1UsersGet) | **Get** /v1/users | 
[**V1UsersIdIssueAuthTokenGet**](UserManagementAPI.md#V1UsersIdIssueAuthTokenGet) | **Get** /v1/users/{id}/issue-auth-token | 



## V1UsersGet

> map[string]interface{} V1UsersGet(ctx).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UserManagementAPI.V1UsersGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserManagementAPI.V1UsersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1UsersGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `UserManagementAPI.V1UsersGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1UsersGetRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1UsersIdIssueAuthTokenGet

> map[string]interface{} V1UsersIdIssueAuthTokenGet(ctx, id).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	id := "id_example" // string | The ID of the user to issue a temporary auth token for

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UserManagementAPI.V1UsersIdIssueAuthTokenGet(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserManagementAPI.V1UsersIdIssueAuthTokenGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1UsersIdIssueAuthTokenGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `UserManagementAPI.V1UsersIdIssueAuthTokenGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | The ID of the user to issue a temporary auth token for | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1UsersIdIssueAuthTokenGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

