# \SystemSettingsAPI

All URIs are relative to *https://raw.githubusercontent.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**V1SystemEnvDumpGet**](SystemSettingsAPI.md#V1SystemEnvDumpGet) | **Get** /v1/system/env-dump | 
[**V1SystemExportChatsGet**](SystemSettingsAPI.md#V1SystemExportChatsGet) | **Get** /v1/system/export-chats | 
[**V1SystemGet**](SystemSettingsAPI.md#V1SystemGet) | **Get** /v1/system | 
[**V1SystemRemoveDocumentsDelete**](SystemSettingsAPI.md#V1SystemRemoveDocumentsDelete) | **Delete** /v1/system/remove-documents | 
[**V1SystemUpdateEnvPost**](SystemSettingsAPI.md#V1SystemUpdateEnvPost) | **Post** /v1/system/update-env | 
[**V1SystemVectorCountGet**](SystemSettingsAPI.md#V1SystemVectorCountGet) | **Get** /v1/system/vector-count | 



## V1SystemEnvDumpGet

> V1SystemEnvDumpGet(ctx).Execute()





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
	r, err := apiClient.SystemSettingsAPI.V1SystemEnvDumpGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemSettingsAPI.V1SystemEnvDumpGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1SystemEnvDumpGetRequest struct via the builder pattern


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


## V1SystemExportChatsGet

> map[string]interface{} V1SystemExportChatsGet(ctx).Type_(type_).Execute()





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
	type_ := "type__example" // string | Export format jsonl, json, csv, jsonAlpaca (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemSettingsAPI.V1SystemExportChatsGet(context.Background()).Type_(type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemSettingsAPI.V1SystemExportChatsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1SystemExportChatsGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `SystemSettingsAPI.V1SystemExportChatsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiV1SystemExportChatsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type_** | **string** | Export format jsonl, json, csv, jsonAlpaca | 

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


## V1SystemGet

> map[string]interface{} V1SystemGet(ctx).Execute()





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
	resp, r, err := apiClient.SystemSettingsAPI.V1SystemGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemSettingsAPI.V1SystemGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1SystemGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `SystemSettingsAPI.V1SystemGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1SystemGetRequest struct via the builder pattern


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


## V1SystemRemoveDocumentsDelete

> map[string]interface{} V1SystemRemoveDocumentsDelete(ctx).V1SystemRemoveDocumentsDeleteRequest(v1SystemRemoveDocumentsDeleteRequest).Execute()





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
	v1SystemRemoveDocumentsDeleteRequest := *openapiclient.NewV1SystemRemoveDocumentsDeleteRequest() // V1SystemRemoveDocumentsDeleteRequest | Array of document names to be removed permanently.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.SystemSettingsAPI.V1SystemRemoveDocumentsDelete(context.Background()).V1SystemRemoveDocumentsDeleteRequest(v1SystemRemoveDocumentsDeleteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemSettingsAPI.V1SystemRemoveDocumentsDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1SystemRemoveDocumentsDelete`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `SystemSettingsAPI.V1SystemRemoveDocumentsDelete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiV1SystemRemoveDocumentsDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **v1SystemRemoveDocumentsDeleteRequest** | [**V1SystemRemoveDocumentsDeleteRequest**](V1SystemRemoveDocumentsDeleteRequest.md) | Array of document names to be removed permanently. | 

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


## V1SystemUpdateEnvPost

> map[string]interface{} V1SystemUpdateEnvPost(ctx).Execute()





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
	resp, r, err := apiClient.SystemSettingsAPI.V1SystemUpdateEnvPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemSettingsAPI.V1SystemUpdateEnvPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1SystemUpdateEnvPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `SystemSettingsAPI.V1SystemUpdateEnvPost`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1SystemUpdateEnvPostRequest struct via the builder pattern


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


## V1SystemVectorCountGet

> map[string]interface{} V1SystemVectorCountGet(ctx).Execute()





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
	resp, r, err := apiClient.SystemSettingsAPI.V1SystemVectorCountGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SystemSettingsAPI.V1SystemVectorCountGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1SystemVectorCountGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `SystemSettingsAPI.V1SystemVectorCountGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1SystemVectorCountGetRequest struct via the builder pattern


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

