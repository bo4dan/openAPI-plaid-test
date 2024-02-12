# PlaidApi.DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**institutionsSearchGet**](DefaultApi.md#institutionsSearchGet) | **GET** /institutions/search | Search institutions



## institutionsSearchGet

> InstitutionsSearchGet200Response institutionsSearchGet(query, opts)

Search institutions

Returns a list of institutions matching the search query

### Example

```javascript
import PlaidApi from 'plaid_api';

let apiInstance = new PlaidApi.DefaultApi();
let query = "query_example"; // String | Search query string
let opts = {
  'products': ["null"] // [String] | Products to filter institutions by
};
apiInstance.institutionsSearchGet(query, opts, (error, data, response) => {
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
 **query** | **String**| Search query string | 
 **products** | [**[String]**](String.md)| Products to filter institutions by | [optional] 

### Return type

[**InstitutionsSearchGet200Response**](InstitutionsSearchGet200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

