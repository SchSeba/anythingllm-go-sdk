# \WorkspacesAPI

All URIs are relative to *https://raw.githubusercontent.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**V1WorkspaceNewPost**](WorkspacesAPI.md#V1WorkspaceNewPost) | **Post** /v1/workspace/new | 
[**V1WorkspaceSlugChatPost**](WorkspacesAPI.md#V1WorkspaceSlugChatPost) | **Post** /v1/workspace/{slug}/chat | 
[**V1WorkspaceSlugChatsGet**](WorkspacesAPI.md#V1WorkspaceSlugChatsGet) | **Get** /v1/workspace/{slug}/chats | 
[**V1WorkspaceSlugDelete**](WorkspacesAPI.md#V1WorkspaceSlugDelete) | **Delete** /v1/workspace/{slug} | 
[**V1WorkspaceSlugGet**](WorkspacesAPI.md#V1WorkspaceSlugGet) | **Get** /v1/workspace/{slug} | 
[**V1WorkspaceSlugStreamChatPost**](WorkspacesAPI.md#V1WorkspaceSlugStreamChatPost) | **Post** /v1/workspace/{slug}/stream-chat | 
[**V1WorkspaceSlugUpdateEmbeddingsPost**](WorkspacesAPI.md#V1WorkspaceSlugUpdateEmbeddingsPost) | **Post** /v1/workspace/{slug}/update-embeddings | 
[**V1WorkspaceSlugUpdatePinPost**](WorkspacesAPI.md#V1WorkspaceSlugUpdatePinPost) | **Post** /v1/workspace/{slug}/update-pin | 
[**V1WorkspaceSlugUpdatePost**](WorkspacesAPI.md#V1WorkspaceSlugUpdatePost) | **Post** /v1/workspace/{slug}/update | 
[**V1WorkspaceSlugVectorSearchPost**](WorkspacesAPI.md#V1WorkspaceSlugVectorSearchPost) | **Post** /v1/workspace/{slug}/vector-search | 
[**V1WorkspacesGet**](WorkspacesAPI.md#V1WorkspacesGet) | **Get** /v1/workspaces | 



## V1WorkspaceNewPost

> map[string]interface{} V1WorkspaceNewPost(ctx).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspaceNewPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceNewPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceNewPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspaceNewPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceNewPostRequest struct via the builder pattern


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


## V1WorkspaceSlugChatPost

> map[string]interface{} V1WorkspaceSlugChatPost(ctx, slug).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {
	slug := "slug_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspaceSlugChatPost(context.Background(), slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceSlugChatPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugChatPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspaceSlugChatPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugChatPostRequest struct via the builder pattern


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


## V1WorkspaceSlugChatsGet

> map[string]interface{} V1WorkspaceSlugChatsGet(ctx, slug).ApiSessionId(apiSessionId).Limit(limit).OrderBy(orderBy).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {
	slug := "slug_example" // string | Unique slug of workspace to find
	apiSessionId := "apiSessionId_example" // string | Optional apiSessionId to filter by (optional)
	limit := int32(56) // int32 | Optional number of chat messages to return (default: 100) (optional)
	orderBy := "orderBy_example" // string | Optional order of chat messages (asc or desc) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspaceSlugChatsGet(context.Background(), slug).ApiSessionId(apiSessionId).Limit(limit).OrderBy(orderBy).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceSlugChatsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugChatsGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspaceSlugChatsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace to find | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugChatsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **apiSessionId** | **string** | Optional apiSessionId to filter by | 
 **limit** | **int32** | Optional number of chat messages to return (default: 100) | 
 **orderBy** | **string** | Optional order of chat messages (asc or desc) | 

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


## V1WorkspaceSlugDelete

> V1WorkspaceSlugDelete(ctx, slug).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {
	slug := "slug_example" // string | Unique slug of workspace to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WorkspacesAPI.V1WorkspaceSlugDelete(context.Background(), slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceSlugDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugDeleteRequest struct via the builder pattern


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


## V1WorkspaceSlugGet

> map[string]interface{} V1WorkspaceSlugGet(ctx, slug).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {
	slug := "slug_example" // string | Unique slug of workspace to find

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspaceSlugGet(context.Background(), slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceSlugGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspaceSlugGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace to find | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugGetRequest struct via the builder pattern


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


## V1WorkspaceSlugStreamChatPost

> []string V1WorkspaceSlugStreamChatPost(ctx, slug).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {
	slug := "slug_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspaceSlugStreamChatPost(context.Background(), slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceSlugStreamChatPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugStreamChatPost`: []string
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspaceSlugStreamChatPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugStreamChatPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


## V1WorkspaceSlugUpdateEmbeddingsPost

> map[string]interface{} V1WorkspaceSlugUpdateEmbeddingsPost(ctx, slug).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {
	slug := "slug_example" // string | Unique slug of workspace to find

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspaceSlugUpdateEmbeddingsPost(context.Background(), slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceSlugUpdateEmbeddingsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugUpdateEmbeddingsPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspaceSlugUpdateEmbeddingsPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace to find | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugUpdateEmbeddingsPostRequest struct via the builder pattern


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


## V1WorkspaceSlugUpdatePinPost

> map[string]interface{} V1WorkspaceSlugUpdatePinPost(ctx, slug).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {
	slug := "slug_example" // string | Unique slug of workspace to find

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspaceSlugUpdatePinPost(context.Background(), slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceSlugUpdatePinPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugUpdatePinPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspaceSlugUpdatePinPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace to find | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugUpdatePinPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1WorkspaceSlugUpdatePost

> map[string]interface{} V1WorkspaceSlugUpdatePost(ctx, slug).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {
	slug := "slug_example" // string | Unique slug of workspace to find

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspaceSlugUpdatePost(context.Background(), slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceSlugUpdatePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugUpdatePost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspaceSlugUpdatePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace to find | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugUpdatePostRequest struct via the builder pattern


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


## V1WorkspaceSlugVectorSearchPost

> map[string]interface{} V1WorkspaceSlugVectorSearchPost(ctx, slug).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {
	slug := "slug_example" // string | Unique slug of workspace to search in

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspaceSlugVectorSearchPost(context.Background(), slug).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspaceSlugVectorSearchPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspaceSlugVectorSearchPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspaceSlugVectorSearchPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Unique slug of workspace to search in | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspaceSlugVectorSearchPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1WorkspacesGet

> map[string]interface{} V1WorkspacesGet(ctx).Execute()





### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/SchSeba/anythingllm-go-sdk"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.V1WorkspacesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.V1WorkspacesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1WorkspacesGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.V1WorkspacesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1WorkspacesGetRequest struct via the builder pattern


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

