# \DocumentsAPI

All URIs are relative to *https://raw.githubusercontent.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**V1DocumentAcceptedFileTypesGet**](DocumentsAPI.md#V1DocumentAcceptedFileTypesGet) | **Get** /v1/document/accepted-file-types | 
[**V1DocumentCreateFolderPost**](DocumentsAPI.md#V1DocumentCreateFolderPost) | **Post** /v1/document/create-folder | 
[**V1DocumentDocNameGet**](DocumentsAPI.md#V1DocumentDocNameGet) | **Get** /v1/document/{docName} | 
[**V1DocumentMetadataSchemaGet**](DocumentsAPI.md#V1DocumentMetadataSchemaGet) | **Get** /v1/document/metadata-schema | 
[**V1DocumentMoveFilesPost**](DocumentsAPI.md#V1DocumentMoveFilesPost) | **Post** /v1/document/move-files | 
[**V1DocumentRawTextPost**](DocumentsAPI.md#V1DocumentRawTextPost) | **Post** /v1/document/raw-text | 
[**V1DocumentRemoveFolderDelete**](DocumentsAPI.md#V1DocumentRemoveFolderDelete) | **Delete** /v1/document/remove-folder | 
[**V1DocumentUploadFolderNamePost**](DocumentsAPI.md#V1DocumentUploadFolderNamePost) | **Post** /v1/document/upload/{folderName} | 
[**V1DocumentUploadLinkPost**](DocumentsAPI.md#V1DocumentUploadLinkPost) | **Post** /v1/document/upload-link | 
[**V1DocumentUploadPost**](DocumentsAPI.md#V1DocumentUploadPost) | **Post** /v1/document/upload | 
[**V1DocumentsFolderFolderNameGet**](DocumentsAPI.md#V1DocumentsFolderFolderNameGet) | **Get** /v1/documents/folder/{folderName} | 
[**V1DocumentsGet**](DocumentsAPI.md#V1DocumentsGet) | **Get** /v1/documents | 



## V1DocumentAcceptedFileTypesGet

> map[string]interface{} V1DocumentAcceptedFileTypesGet(ctx).Execute()





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
	resp, r, err := apiClient.DocumentsAPI.V1DocumentAcceptedFileTypesGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentAcceptedFileTypesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentAcceptedFileTypesGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentAcceptedFileTypesGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentAcceptedFileTypesGetRequest struct via the builder pattern


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


## V1DocumentCreateFolderPost

> map[string]interface{} V1DocumentCreateFolderPost(ctx).Body(body).Execute()





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
	body := "body_example" // string | Name of the folder to create.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.V1DocumentCreateFolderPost(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentCreateFolderPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentCreateFolderPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentCreateFolderPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentCreateFolderPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **string** | Name of the folder to create. | 

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


## V1DocumentDocNameGet

> map[string]interface{} V1DocumentDocNameGet(ctx, docName).Execute()





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
	docName := "docName_example" // string | Unique document name to find (name in /documents)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.V1DocumentDocNameGet(context.Background(), docName).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentDocNameGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentDocNameGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentDocNameGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**docName** | **string** | Unique document name to find (name in /documents) | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentDocNameGetRequest struct via the builder pattern


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


## V1DocumentMetadataSchemaGet

> map[string]interface{} V1DocumentMetadataSchemaGet(ctx).Execute()





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
	resp, r, err := apiClient.DocumentsAPI.V1DocumentMetadataSchemaGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentMetadataSchemaGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentMetadataSchemaGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentMetadataSchemaGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentMetadataSchemaGetRequest struct via the builder pattern


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


## V1DocumentMoveFilesPost

> map[string]interface{} V1DocumentMoveFilesPost(ctx).Body(body).Execute()





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
	body := map[string]interface{}{ ... } // map[string]interface{} | Array of objects containing source and destination paths of files to move.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.V1DocumentMoveFilesPost(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentMoveFilesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentMoveFilesPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentMoveFilesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentMoveFilesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **map[string]interface{}** | Array of objects containing source and destination paths of files to move. | 

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


## V1DocumentRawTextPost

> map[string]interface{} V1DocumentRawTextPost(ctx).Body(body).Execute()





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
	body := map[string]interface{}{ ... } // map[string]interface{} | Text content and metadata of the file to be saved to the system. Use metadata-schema endpoint to get the possible metadata keys

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.V1DocumentRawTextPost(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentRawTextPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentRawTextPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentRawTextPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentRawTextPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **map[string]interface{}** | Text content and metadata of the file to be saved to the system. Use metadata-schema endpoint to get the possible metadata keys | 

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


## V1DocumentRemoveFolderDelete

> map[string]interface{} V1DocumentRemoveFolderDelete(ctx).V1DocumentRemoveFolderDeleteRequest(v1DocumentRemoveFolderDeleteRequest).Execute()





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
	v1DocumentRemoveFolderDeleteRequest := *openapiclient.NewV1DocumentRemoveFolderDeleteRequest() // V1DocumentRemoveFolderDeleteRequest | Name of the folder to remove.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.V1DocumentRemoveFolderDelete(context.Background()).V1DocumentRemoveFolderDeleteRequest(v1DocumentRemoveFolderDeleteRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentRemoveFolderDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentRemoveFolderDelete`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentRemoveFolderDelete`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentRemoveFolderDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **v1DocumentRemoveFolderDeleteRequest** | [**V1DocumentRemoveFolderDeleteRequest**](V1DocumentRemoveFolderDeleteRequest.md) | Name of the folder to remove. | 

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


## V1DocumentUploadFolderNamePost

> map[string]interface{} V1DocumentUploadFolderNamePost(ctx, folderName).File(file).AddToWorkspaces(addToWorkspaces).Execute()





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
	folderName := "my-folder" // string | Target folder path (defaults to 'custom-documents' if not provided)
	file := os.NewFile(1234, "some_file") // *os.File | The file to upload
	addToWorkspaces := "addToWorkspaces_example" // string | comma-separated text-string of workspace slugs to embed the document into post-upload. eg: workspace1,workspace2 (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.V1DocumentUploadFolderNamePost(context.Background(), folderName).File(file).AddToWorkspaces(addToWorkspaces).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentUploadFolderNamePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentUploadFolderNamePost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentUploadFolderNamePost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**folderName** | **string** | Target folder path (defaults to &#39;custom-documents&#39; if not provided) | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentUploadFolderNamePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **file** | ***os.File** | The file to upload | 
 **addToWorkspaces** | **string** | comma-separated text-string of workspace slugs to embed the document into post-upload. eg: workspace1,workspace2 | 

### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1DocumentUploadLinkPost

> map[string]interface{} V1DocumentUploadLinkPost(ctx).Body(body).Execute()





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
	body := map[string]interface{}{ ... } // map[string]interface{} | Link of web address to be scraped and optionally a comma-separated list of workspace slugs to embed the document into post-upload.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.V1DocumentUploadLinkPost(context.Background()).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentUploadLinkPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentUploadLinkPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentUploadLinkPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentUploadLinkPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **map[string]interface{}** | Link of web address to be scraped and optionally a comma-separated list of workspace slugs to embed the document into post-upload. | 

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


## V1DocumentUploadPost

> map[string]interface{} V1DocumentUploadPost(ctx).File(file).AddToWorkspaces(addToWorkspaces).Execute()





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
	file := os.NewFile(1234, "some_file") // *os.File | The file to upload
	addToWorkspaces := "addToWorkspaces_example" // string | comma-separated text-string of workspace slugs to embed the document into post-upload. eg: workspace1,workspace2 (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.V1DocumentUploadPost(context.Background()).File(file).AddToWorkspaces(addToWorkspaces).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentUploadPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentUploadPost`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentUploadPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentUploadPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **file** | ***os.File** | The file to upload | 
 **addToWorkspaces** | **string** | comma-separated text-string of workspace slugs to embed the document into post-upload. eg: workspace1,workspace2 | 

### Return type

**map[string]interface{}**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json, application/xml

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## V1DocumentsFolderFolderNameGet

> map[string]interface{} V1DocumentsFolderFolderNameGet(ctx, folderName).Execute()





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
	folderName := "folderName_example" // string | Name of the folder to retrieve documents from

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DocumentsAPI.V1DocumentsFolderFolderNameGet(context.Background(), folderName).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentsFolderFolderNameGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentsFolderFolderNameGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentsFolderFolderNameGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**folderName** | **string** | Name of the folder to retrieve documents from | 

### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentsFolderFolderNameGetRequest struct via the builder pattern


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


## V1DocumentsGet

> map[string]interface{} V1DocumentsGet(ctx).Execute()





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
	resp, r, err := apiClient.DocumentsAPI.V1DocumentsGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DocumentsAPI.V1DocumentsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `V1DocumentsGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `DocumentsAPI.V1DocumentsGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiV1DocumentsGetRequest struct via the builder pattern


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

