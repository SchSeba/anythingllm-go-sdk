# \AdminAPI

All URIs are relative to *https://raw.githubusercontent.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**V1AdminInviteIdDelete**](AdminAPI.md#V1AdminInviteIdDelete) | **Delete** /v1/admin/invite/{id} | 
[**V1AdminInviteNewPost**](AdminAPI.md#V1AdminInviteNewPost) | **Post** /v1/admin/invite/new | 
[**V1AdminInvitesGet**](AdminAPI.md#V1AdminInvitesGet) | **Get** /v1/admin/invites | 
[**V1AdminIsMultiUserModeGet**](AdminAPI.md#V1AdminIsMultiUserModeGet) | **Get** /v1/admin/is-multi-user-mode | 
[**V1AdminPreferencesPost**](AdminAPI.md#V1AdminPreferencesPost) | **Post** /v1/admin/preferences | 
[**V1AdminUsersGet**](AdminAPI.md#V1AdminUsersGet) | **Get** /v1/admin/users | 
[**V1AdminUsersIdDelete**](AdminAPI.md#V1AdminUsersIdDelete) | **Delete** /v1/admin/users/{id} | 
[**V1AdminUsersIdPost**](AdminAPI.md#V1AdminUsersIdPost) | **Post** /v1/admin/users/{id} | 
[**V1AdminUsersNewPost**](AdminAPI.md#V1AdminUsersNewPost) | **Post** /v1/admin/users/new | 
[**V1AdminWorkspaceChatsPost**](AdminAPI.md#V1AdminWorkspaceChatsPost) | **Post** /v1/admin/workspace-chats | 
[**V1AdminWorkspacesWorkspaceIdUpdateUsersPost**](AdminAPI.md#V1AdminWorkspacesWorkspaceIdUpdateUsersPost) | **Post** /v1/admin/workspaces/{workspaceId}/update-users | 
[**V1AdminWorkspacesWorkspaceIdUsersGet**](AdminAPI.md#V1AdminWorkspacesWorkspaceIdUsersGet) | **Get** /v1/admin/workspaces/{workspaceId}/users | 
[**V1AdminWorkspacesWorkspaceSlugManageUsersPost**](AdminAPI.md#V1AdminWorkspacesWorkspaceSlugManageUsersPost) | **Post** /v1/admin/workspaces/{workspaceSlug}/manage-users | 



## V1AdminInviteIdDelete

> map[string]interface{} V1AdminInviteIdDelete(ctx, id).Execute()





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
	id := "id_example" // string | id of the invite in the database.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdminAPI.V1AdminInviteIdDelete(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminInviteIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminInviteIdDelete`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminInviteIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | id of the invite in the database. | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminInviteIdDeleteRequest struct via the builder pattern


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


## V1AdminInviteNewPost

> map[string]interface{} V1AdminInviteNewPost(ctx).Execute()





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
	resp, r, err := apiClient.AdminAPI.V1AdminInviteNewPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminInviteNewPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminInviteNewPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminInviteNewPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminInviteNewPostRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1AdminInvitesGet

> map[string]interface{} V1AdminInvitesGet(ctx).Execute()





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
	resp, r, err := apiClient.AdminAPI.V1AdminInvitesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminInvitesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminInvitesGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminInvitesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminInvitesGetRequest struct via the builder pattern


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


## V1AdminIsMultiUserModeGet

> map[string]interface{} V1AdminIsMultiUserModeGet(ctx).Execute()





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
	resp, r, err := apiClient.AdminAPI.V1AdminIsMultiUserModeGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminIsMultiUserModeGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminIsMultiUserModeGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminIsMultiUserModeGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminIsMultiUserModeGetRequest struct via the builder pattern


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


## V1AdminPreferencesPost

> map[string]interface{} V1AdminPreferencesPost(ctx).Execute()





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
	resp, r, err := apiClient.AdminAPI.V1AdminPreferencesPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminPreferencesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminPreferencesPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminPreferencesPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminPreferencesPostRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1AdminUsersGet

> map[string]interface{} V1AdminUsersGet(ctx).Execute()





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
	resp, r, err := apiClient.AdminAPI.V1AdminUsersGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminUsersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminUsersGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminUsersGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminUsersGetRequest struct via the builder pattern


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


## V1AdminUsersIdDelete

> map[string]interface{} V1AdminUsersIdDelete(ctx, id).Execute()





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
	id := "id_example" // string | id of the user in the database.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdminAPI.V1AdminUsersIdDelete(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminUsersIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminUsersIdDelete`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminUsersIdDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | id of the user in the database. | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminUsersIdDeleteRequest struct via the builder pattern


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


## V1AdminUsersIdPost

> map[string]interface{} V1AdminUsersIdPost(ctx, id).Execute()





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
	id := "id_example" // string | id of the user in the database.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdminAPI.V1AdminUsersIdPost(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminUsersIdPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminUsersIdPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminUsersIdPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | id of the user in the database. | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminUsersIdPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1AdminUsersNewPost

> map[string]interface{} V1AdminUsersNewPost(ctx).Execute()





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
	resp, r, err := apiClient.AdminAPI.V1AdminUsersNewPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminUsersNewPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminUsersNewPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminUsersNewPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminUsersNewPostRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1AdminWorkspaceChatsPost

> map[string]interface{} V1AdminWorkspaceChatsPost(ctx).Execute()





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
	resp, r, err := apiClient.AdminAPI.V1AdminWorkspaceChatsPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminWorkspaceChatsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminWorkspaceChatsPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminWorkspaceChatsPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminWorkspaceChatsPostRequest struct via the builder pattern


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1AdminWorkspacesWorkspaceIdUpdateUsersPost

> map[string]interface{} V1AdminWorkspacesWorkspaceIdUpdateUsersPost(ctx, workspaceId).Execute()





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
	workspaceId := "workspaceId_example" // string | id of the workspace in the database.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdminAPI.V1AdminWorkspacesWorkspaceIdUpdateUsersPost(context.Background(), workspaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminWorkspacesWorkspaceIdUpdateUsersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminWorkspacesWorkspaceIdUpdateUsersPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminWorkspacesWorkspaceIdUpdateUsersPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** | id of the workspace in the database. | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminWorkspacesWorkspaceIdUpdateUsersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1AdminWorkspacesWorkspaceIdUsersGet

> map[string]interface{} V1AdminWorkspacesWorkspaceIdUsersGet(ctx, workspaceId).Execute()





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
	workspaceId := "workspaceId_example" // string | id of the workspace.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdminAPI.V1AdminWorkspacesWorkspaceIdUsersGet(context.Background(), workspaceId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminWorkspacesWorkspaceIdUsersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminWorkspacesWorkspaceIdUsersGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminWorkspacesWorkspaceIdUsersGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceId** | **string** | id of the workspace. | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminWorkspacesWorkspaceIdUsersGetRequest struct via the builder pattern


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


## V1AdminWorkspacesWorkspaceSlugManageUsersPost

> map[string]interface{} V1AdminWorkspacesWorkspaceSlugManageUsersPost(ctx, workspaceSlug).Execute()





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
	workspaceSlug := "workspaceSlug_example" // string | slug of the workspace in the database

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AdminAPI.V1AdminWorkspacesWorkspaceSlugManageUsersPost(context.Background(), workspaceSlug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AdminAPI.V1AdminWorkspacesWorkspaceSlugManageUsersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1AdminWorkspacesWorkspaceSlugManageUsersPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `AdminAPI.V1AdminWorkspacesWorkspaceSlugManageUsersPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**workspaceSlug** | **string** | slug of the workspace in the database | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1AdminWorkspacesWorkspaceSlugManageUsersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

