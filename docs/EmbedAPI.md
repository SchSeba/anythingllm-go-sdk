# \EmbedAPI

All URIs are relative to *https://raw.githubusercontent.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**V1EmbedEmbedUuidChatsGet**](EmbedAPI.md#V1EmbedEmbedUuidChatsGet) | **Get** /v1/embed/{embedUuid}/chats | 
[**V1EmbedEmbedUuidChatsSessionUuidGet**](EmbedAPI.md#V1EmbedEmbedUuidChatsSessionUuidGet) | **Get** /v1/embed/{embedUuid}/chats/{sessionUuid} | 
[**V1EmbedEmbedUuidDelete**](EmbedAPI.md#V1EmbedEmbedUuidDelete) | **Delete** /v1/embed/{embedUuid} | 
[**V1EmbedEmbedUuidPost**](EmbedAPI.md#V1EmbedEmbedUuidPost) | **Post** /v1/embed/{embedUuid} | 
[**V1EmbedGet**](EmbedAPI.md#V1EmbedGet) | **Get** /v1/embed | 
[**V1EmbedNewPost**](EmbedAPI.md#V1EmbedNewPost) | **Post** /v1/embed/new | 



## V1EmbedEmbedUuidChatsGet

> map[string]interface{} V1EmbedEmbedUuidChatsGet(ctx, embedUuid).Execute()





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
	embedUuid := "embedUuid_example" // string | UUID of the embed

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmbedAPI.V1EmbedEmbedUuidChatsGet(context.Background(), embedUuid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmbedAPI.V1EmbedEmbedUuidChatsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1EmbedEmbedUuidChatsGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `EmbedAPI.V1EmbedEmbedUuidChatsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**embedUuid** | **string** | UUID of the embed | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1EmbedEmbedUuidChatsGetRequest struct via the builder pattern


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


## V1EmbedEmbedUuidChatsSessionUuidGet

> map[string]interface{} V1EmbedEmbedUuidChatsSessionUuidGet(ctx, embedUuid, sessionUuid).Execute()





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
	embedUuid := "embedUuid_example" // string | UUID of the embed
	sessionUuid := "sessionUuid_example" // string | UUID of the session

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmbedAPI.V1EmbedEmbedUuidChatsSessionUuidGet(context.Background(), embedUuid, sessionUuid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmbedAPI.V1EmbedEmbedUuidChatsSessionUuidGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1EmbedEmbedUuidChatsSessionUuidGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `EmbedAPI.V1EmbedEmbedUuidChatsSessionUuidGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**embedUuid** | **string** | UUID of the embed | 
**sessionUuid** | **string** | UUID of the session | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1EmbedEmbedUuidChatsSessionUuidGetRequest struct via the builder pattern


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


## V1EmbedEmbedUuidDelete

> map[string]interface{} V1EmbedEmbedUuidDelete(ctx, embedUuid).Execute()





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
	embedUuid := "embedUuid_example" // string | UUID of the embed to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmbedAPI.V1EmbedEmbedUuidDelete(context.Background(), embedUuid).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmbedAPI.V1EmbedEmbedUuidDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1EmbedEmbedUuidDelete`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `EmbedAPI.V1EmbedEmbedUuidDelete`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**embedUuid** | **string** | UUID of the embed to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1EmbedEmbedUuidDeleteRequest struct via the builder pattern


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


## V1EmbedEmbedUuidPost

> map[string]interface{} V1EmbedEmbedUuidPost(ctx, embedUuid).Body(body).Execute()





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
	embedUuid := "embedUuid_example" // string | UUID of the embed to update
	body := map[string]interface{}{ ... } // map[string]interface{} | JSON object containing embed configuration updates

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmbedAPI.V1EmbedEmbedUuidPost(context.Background(), embedUuid).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmbedAPI.V1EmbedEmbedUuidPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1EmbedEmbedUuidPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `EmbedAPI.V1EmbedEmbedUuidPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**embedUuid** | **string** | UUID of the embed to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1EmbedEmbedUuidPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | **map[string]interface{}** | JSON object containing embed configuration updates | 

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


## V1EmbedGet

> map[string]interface{} V1EmbedGet(ctx).Execute()





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
	resp, r, err := apiClient.EmbedAPI.V1EmbedGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmbedAPI.V1EmbedGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1EmbedGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `EmbedAPI.V1EmbedGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1EmbedGetRequest struct via the builder pattern


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


## V1EmbedNewPost

> map[string]interface{} V1EmbedNewPost(ctx).Body(body).Execute()





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
	body := map[string]interface{}{ ... } // map[string]interface{} | JSON object containing embed configuration details

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EmbedAPI.V1EmbedNewPost(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EmbedAPI.V1EmbedNewPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1EmbedNewPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `EmbedAPI.V1EmbedNewPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiV1EmbedNewPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **map[string]interface{}** | JSON object containing embed configuration details | 

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

