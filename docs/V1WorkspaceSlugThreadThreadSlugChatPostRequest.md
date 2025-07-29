# V1WorkspaceSlugThreadThreadSlugChatPostRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | **string** | The message/prompt to send to the workspace thread | 
**Mode** | Pointer to **string** | The type of conversation - query or chat | [optional] [default to "query"]
**UserId** | Pointer to **NullableInt32** | Optional user ID associated with the chat | [optional] 
**Attachments** | Pointer to [**[]V1WorkspaceSlugThreadThreadSlugChatPostRequestAttachmentsInner**](V1WorkspaceSlugThreadThreadSlugChatPostRequestAttachmentsInner.md) | Optional array of file attachments | [optional] [default to []]
**Reset** | Pointer to **bool** | Whether to reset the conversation thread | [optional] [default to false]

## Methods

### NewV1WorkspaceSlugThreadThreadSlugChatPostRequest

`func NewV1WorkspaceSlugThreadThreadSlugChatPostRequest(message string, ) *V1WorkspaceSlugThreadThreadSlugChatPostRequest`

NewV1WorkspaceSlugThreadThreadSlugChatPostRequest instantiates a new V1WorkspaceSlugThreadThreadSlugChatPostRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewV1WorkspaceSlugThreadThreadSlugChatPostRequestWithDefaults

`func NewV1WorkspaceSlugThreadThreadSlugChatPostRequestWithDefaults() *V1WorkspaceSlugThreadThreadSlugChatPostRequest`

NewV1WorkspaceSlugThreadThreadSlugChatPostRequestWithDefaults instantiates a new V1WorkspaceSlugThreadThreadSlugChatPostRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetMode

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetMode() string`

GetMode returns the Mode field if non-nil, zero value otherwise.

### GetModeOk

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetModeOk() (*string, bool)`

GetModeOk returns a tuple with the Mode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMode

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) SetMode(v string)`

SetMode sets Mode field to given value.

### HasMode

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) HasMode() bool`

HasMode returns a boolean if a field has been set.

### GetUserId

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetUserId() int32`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetUserIdOk() (*int32, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) SetUserId(v int32)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### SetUserIdNil

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) SetUserIdNil(b bool)`

 SetUserIdNil sets the value for UserId to be an explicit nil

### UnsetUserId
`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) UnsetUserId()`

UnsetUserId ensures that no value is present for UserId, not even an explicit nil
### GetAttachments

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetAttachments() []V1WorkspaceSlugThreadThreadSlugChatPostRequestAttachmentsInner`

GetAttachments returns the Attachments field if non-nil, zero value otherwise.

### GetAttachmentsOk

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetAttachmentsOk() (*[]V1WorkspaceSlugThreadThreadSlugChatPostRequestAttachmentsInner, bool)`

GetAttachmentsOk returns a tuple with the Attachments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttachments

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) SetAttachments(v []V1WorkspaceSlugThreadThreadSlugChatPostRequestAttachmentsInner)`

SetAttachments sets Attachments field to given value.

### HasAttachments

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) HasAttachments() bool`

HasAttachments returns a boolean if a field has been set.

### GetReset

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetReset() bool`

GetReset returns the Reset field if non-nil, zero value otherwise.

### GetResetOk

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) GetResetOk() (*bool, bool)`

GetResetOk returns a tuple with the Reset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReset

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) SetReset(v bool)`

SetReset sets Reset field to given value.

### HasReset

`func (o *V1WorkspaceSlugThreadThreadSlugChatPostRequest) HasReset() bool`

HasReset returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


