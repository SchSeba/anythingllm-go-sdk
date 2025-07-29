# \OpenAICompatibleEndpointsAPI

All URIs are relative to *https://raw.githubusercontent.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**V1OpenaiChatCompletionsPost**](OpenAICompatibleEndpointsAPI.md#V1OpenaiChatCompletionsPost) | **Post** /v1/openai/chat/completions | 
[**V1OpenaiEmbeddingsPost**](OpenAICompatibleEndpointsAPI.md#V1OpenaiEmbeddingsPost) | **Post** /v1/openai/embeddings | 
[**V1OpenaiModelsGet**](OpenAICompatibleEndpointsAPI.md#V1OpenaiModelsGet) | **Get** /v1/openai/models | 
[**V1OpenaiVectorStoresGet**](OpenAICompatibleEndpointsAPI.md#V1OpenaiVectorStoresGet) | **Get** /v1/openai/vector_stores | 



## V1OpenaiChatCompletionsPost

> V1OpenaiChatCompletionsPost(ctx).Execute()





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
	r, err := apiClient.OpenAICompatibleEndpointsAPI.V1OpenaiChatCompletionsPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OpenAICompatibleEndpointsAPI.V1OpenaiChatCompletionsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1OpenaiChatCompletionsPostRequest struct via the builder pattern


### Return type

 (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1OpenaiEmbeddingsPost

> V1OpenaiEmbeddingsPost(ctx).Execute()





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
	r, err := apiClient.OpenAICompatibleEndpointsAPI.V1OpenaiEmbeddingsPost(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OpenAICompatibleEndpointsAPI.V1OpenaiEmbeddingsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1OpenaiEmbeddingsPostRequest struct via the builder pattern


### Return type

 (empty response body)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1OpenaiModelsGet

> map[string]interface{} V1OpenaiModelsGet(ctx).Execute()





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
	resp, r, err := apiClient.OpenAICompatibleEndpointsAPI.V1OpenaiModelsGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OpenAICompatibleEndpointsAPI.V1OpenaiModelsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1OpenaiModelsGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OpenAICompatibleEndpointsAPI.V1OpenaiModelsGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1OpenaiModelsGetRequest struct via the builder pattern


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


## V1OpenaiVectorStoresGet

> map[string]interface{} V1OpenaiVectorStoresGet(ctx).Execute()





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
	resp, r, err := apiClient.OpenAICompatibleEndpointsAPI.V1OpenaiVectorStoresGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OpenAICompatibleEndpointsAPI.V1OpenaiVectorStoresGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1OpenaiVectorStoresGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `OpenAICompatibleEndpointsAPI.V1OpenaiVectorStoresGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1OpenaiVectorStoresGetRequest struct via the builder pattern


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

