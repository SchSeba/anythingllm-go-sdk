# \WorkspaceThreadsAPI

All URIs are relative to *https://raw.githubusercontent.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**V1WorkspaceSlugThreadNewPost**](WorkspaceThreadsAPI.md#V1WorkspaceSlugThreadNewPost) | **Post** /v1/workspace/{slug}/thread/new | 
[**V1WorkspaceSlugThreadThreadSlugChatPost**](WorkspaceThreadsAPI.md#V1WorkspaceSlugThreadThreadSlugChatPost) | **Post** /v1/workspace/{slug}/thread/{threadSlug}/chat | 
[**V1WorkspaceSlugThreadThreadSlugChatsGet**](WorkspaceThreadsAPI.md#V1WorkspaceSlugThreadThreadSlugChatsGet) | **Get** /v1/workspace/{slug}/thread/{threadSlug}/chats | 
[**V1WorkspaceSlugThreadThreadSlugDelete**](WorkspaceThreadsAPI.md#V1WorkspaceSlugThreadThreadSlugDelete) | **Delete** /v1/workspace/{slug}/thread/{threadSlug} | 
[**V1WorkspaceSlugThreadThreadSlugStreamChatPost**](WorkspaceThreadsAPI.md#V1WorkspaceSlugThreadThreadSlugStreamChatPost) | **Post** /v1/workspace/{slug}/thread/{threadSlug}/stream-chat | 
[**V1WorkspaceSlugThreadThreadSlugUpdatePost**](WorkspaceThreadsAPI.md#V1WorkspaceSlugThreadThreadSlugUpdatePost) | **Post** /v1/workspace/{slug}/thread/{threadSlug}/update | 



## V1WorkspaceSlugThreadNewPost

> map[string]interface{} V1WorkspaceSlugThreadNewPost(ctx, slug).Execute()





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
	slug := "slug_example" // string | Unique slug of workspace

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspaceThreadsAPI.V1WorkspaceSlugThreadNewPost(context.Background(), slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspaceThreadsAPI.V1WorkspaceSlugThreadNewPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugThreadNewPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspaceThreadsAPI.V1WorkspaceSlugThreadNewPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugThreadNewPostRequest struct via the builder pattern


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


## V1WorkspaceSlugThreadThreadSlugChatPost

> map[string]interface{} V1WorkspaceSlugThreadThreadSlugChatPost(ctx, slug, threadSlug).V1WorkspaceSlugThreadThreadSlugChatPostRequest(v1WorkspaceSlugThreadThreadSlugChatPostRequest).Execute()





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
	slug := "slug_example" // string | Unique slug of workspace
	threadSlug := "threadSlug_example" // string | Unique slug of thread
	v1WorkspaceSlugThreadThreadSlugChatPostRequest := *openapiclient.NewV1WorkspaceSlugThreadThreadSlugChatPostRequest("Message_example") // V1WorkspaceSlugThreadThreadSlugChatPostRequest | Send a prompt to the workspace thread and the type of conversation (query or chat).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugChatPost(context.Background(), slug, threadSlug).V1WorkspaceSlugThreadThreadSlugChatPostRequest(v1WorkspaceSlugThreadThreadSlugChatPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugChatPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugThreadThreadSlugChatPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugChatPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace | 
**threadSlug** | **string** | Unique slug of thread | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugThreadThreadSlugChatPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **v1WorkspaceSlugThreadThreadSlugChatPostRequest** | [**V1WorkspaceSlugThreadThreadSlugChatPostRequest**](V1WorkspaceSlugThreadThreadSlugChatPostRequest.md) | Send a prompt to the workspace thread and the type of conversation (query or chat). | 

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


## V1WorkspaceSlugThreadThreadSlugChatsGet

> map[string]interface{} V1WorkspaceSlugThreadThreadSlugChatsGet(ctx, slug, threadSlug).Execute()





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
	slug := "slug_example" // string | Unique slug of workspace
	threadSlug := "threadSlug_example" // string | Unique slug of thread

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugChatsGet(context.Background(), slug, threadSlug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugChatsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugThreadThreadSlugChatsGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugChatsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace | 
**threadSlug** | **string** | Unique slug of thread | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugThreadThreadSlugChatsGetRequest struct via the builder pattern


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


## V1WorkspaceSlugThreadThreadSlugDelete

> V1WorkspaceSlugThreadThreadSlugDelete(ctx, slug, threadSlug).Execute()





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
	slug := "slug_example" // string | Unique slug of workspace
	threadSlug := "threadSlug_example" // string | Unique slug of thread

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugDelete(context.Background(), slug, threadSlug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace | 
**threadSlug** | **string** | Unique slug of thread | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugThreadThreadSlugDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

 (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1WorkspaceSlugThreadThreadSlugStreamChatPost

> []string V1WorkspaceSlugThreadThreadSlugStreamChatPost(ctx, slug, threadSlug).V1WorkspaceSlugThreadThreadSlugChatPostRequest(v1WorkspaceSlugThreadThreadSlugChatPostRequest).Execute()





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
	slug := "slug_example" // string | Unique slug of workspace
	threadSlug := "threadSlug_example" // string | Unique slug of thread
	v1WorkspaceSlugThreadThreadSlugChatPostRequest := *openapiclient.NewV1WorkspaceSlugThreadThreadSlugChatPostRequest("Message_example") // V1WorkspaceSlugThreadThreadSlugChatPostRequest | Send a prompt to the workspace thread and the type of conversation (query or chat).

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugStreamChatPost(context.Background(), slug, threadSlug).V1WorkspaceSlugThreadThreadSlugChatPostRequest(v1WorkspaceSlugThreadThreadSlugChatPostRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugStreamChatPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugThreadThreadSlugStreamChatPost`: []string
	fmt.Fprintf(os.Stdout, "Response from `WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugStreamChatPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace | 
**threadSlug** | **string** | Unique slug of thread | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugThreadThreadSlugStreamChatPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **v1WorkspaceSlugThreadThreadSlugChatPostRequest** | [**V1WorkspaceSlugThreadThreadSlugChatPostRequest**](V1WorkspaceSlugThreadThreadSlugChatPostRequest.md) | Send a prompt to the workspace thread and the type of conversation (query or chat). | 

### Return type

**[]string**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/event-stream, application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1WorkspaceSlugThreadThreadSlugUpdatePost

> map[string]interface{} V1WorkspaceSlugThreadThreadSlugUpdatePost(ctx, slug, threadSlug).Execute()





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
	slug := "slug_example" // string | Unique slug of workspace
	threadSlug := "threadSlug_example" // string | Unique slug of thread

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugUpdatePost(context.Background(), slug, threadSlug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugUpdatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugThreadThreadSlugUpdatePost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspaceThreadsAPI.V1WorkspaceSlugThreadThreadSlugUpdatePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace | 
**threadSlug** | **string** | Unique slug of thread | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugThreadThreadSlugUpdatePostRequest struct via the builder pattern


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

