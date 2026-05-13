# LthnApi.SystemApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getHealth**](SystemApi.md#getHealth) | **GET** /health | Health check



## getHealth

> GetHealth200Response getHealth()

Health check

Returns server health status

### Example

```javascript
import LthnApi from 'lthn_api';

let apiInstance = new LthnApi.SystemApi();
apiInstance.getHealth((error, data, response) => {
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

[**GetHealth200Response**](GetHealth200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

