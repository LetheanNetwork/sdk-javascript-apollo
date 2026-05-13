# LthnApi.RunnerApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getV1RunnerModels**](RunnerApi.md#getV1RunnerModels) | **GET** /v1/runner/models | List configured runner model routes
[**postV1RunnerChat**](RunnerApi.md#postV1RunnerChat) | **POST** /v1/runner/chat | Multi-turn chat completion
[**postV1RunnerGenerate**](RunnerApi.md#postV1RunnerGenerate) | **POST** /v1/runner/generate | Single-prompt generation



## getV1RunnerModels

> GetV1RunnerModels200Response getV1RunnerModels()

List configured runner model routes



### Example

```javascript
import LthnApi from 'lthn_api';
let defaultClient = LthnApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new LthnApi.RunnerApi();
apiInstance.getV1RunnerModels((error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetV1RunnerModels200Response**](GetV1RunnerModels200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## postV1RunnerChat

> PostV1RunnerChat200Response postV1RunnerChat(postV1RunnerChatRequest)

Multi-turn chat completion



### Example

```javascript
import LthnApi from 'lthn_api';
let defaultClient = LthnApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new LthnApi.RunnerApi();
let postV1RunnerChatRequest = new LthnApi.PostV1RunnerChatRequest(); // PostV1RunnerChatRequest | 
apiInstance.postV1RunnerChat(postV1RunnerChatRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **postV1RunnerChatRequest** | [**PostV1RunnerChatRequest**](PostV1RunnerChatRequest.md)|  | 

### Return type

[**PostV1RunnerChat200Response**](PostV1RunnerChat200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## postV1RunnerGenerate

> PostV1RunnerChat200Response postV1RunnerGenerate(postV1RunnerGenerateRequest)

Single-prompt generation



### Example

```javascript
import LthnApi from 'lthn_api';
let defaultClient = LthnApi.ApiClient.instance;
// Configure Bearer (JWT) access token for authorization: bearerAuth
let bearerAuth = defaultClient.authentications['bearerAuth'];
bearerAuth.accessToken = "YOUR ACCESS TOKEN"

let apiInstance = new LthnApi.RunnerApi();
let postV1RunnerGenerateRequest = new LthnApi.PostV1RunnerGenerateRequest(); // PostV1RunnerGenerateRequest | 
apiInstance.postV1RunnerGenerate(postV1RunnerGenerateRequest, (error, data, response) => {
  if (error) {
    console.error(error);
  } else {
    console.log('API called successfully. Returned data: ' + data);
  }
});
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **postV1RunnerGenerateRequest** | [**PostV1RunnerGenerateRequest**](PostV1RunnerGenerateRequest.md)|  | 

### Return type

[**PostV1RunnerChat200Response**](PostV1RunnerChat200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

