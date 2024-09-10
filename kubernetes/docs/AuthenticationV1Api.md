# Kubernetes::AuthenticationV1Api

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_token_review**](AuthenticationV1Api.md#create_token_review) | **POST** /apis/authentication.k8s.io/v1/tokenreviews |  |
| [**get_api_resources**](AuthenticationV1Api.md#get_api_resources) | **GET** /apis/authentication.k8s.io/v1/ |  |


## create_token_review

> <V1TokenReview> create_token_review(body, opts)



create a TokenReview

### Examples

```ruby
require 'time'
require 'kubernetes-io'
# setup authorization
Kubernetes.configure do |config|
  # Configure API key authorization: BearerToken
  config.api_key['BearerToken'] = 'YOUR API KEY'
  # Uncomment the following line to set a prefix for the API key, e.g. 'Bearer' (defaults to nil)
  # config.api_key_prefix['BearerToken'] = 'Bearer'
end

api_instance = Kubernetes::AuthenticationV1Api.new
body = Kubernetes::V1TokenReview.new({spec: Kubernetes::V1TokenReviewSpec.new}) # V1TokenReview | 
opts = {
  dry_run: 'dry_run_example', # String | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed
  include_uninitialized: true, # Boolean | If IncludeUninitialized is specified, the object may be returned without completing initialization.
  pretty: 'pretty_example' # String | If 'true', then the output is pretty printed.
}

begin
  
  result = api_instance.create_token_review(body, opts)
  p result
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthenticationV1Api->create_token_review: #{e}"
end
```

#### Using the create_token_review_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<V1TokenReview>, Integer, Hash)> create_token_review_with_http_info(body, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.create_token_review_with_http_info(body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <V1TokenReview>
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthenticationV1Api->create_token_review_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **body** | [**V1TokenReview**](V1TokenReview.md) |  |  |
| **dry_run** | **String** | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] |
| **include_uninitialized** | **Boolean** | If IncludeUninitialized is specified, the object may be returned without completing initialization. | [optional] |
| **pretty** | **String** | If &#39;true&#39;, then the output is pretty printed. | [optional] |

### Return type

[**V1TokenReview**](V1TokenReview.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf


## get_api_resources

> <V1APIResourceList> get_api_resources



get available resources

### Examples

```ruby
require 'time'
require 'kubernetes-io'
# setup authorization
Kubernetes.configure do |config|
  # Configure API key authorization: BearerToken
  config.api_key['BearerToken'] = 'YOUR API KEY'
  # Uncomment the following line to set a prefix for the API key, e.g. 'Bearer' (defaults to nil)
  # config.api_key_prefix['BearerToken'] = 'Bearer'
end

api_instance = Kubernetes::AuthenticationV1Api.new

begin
  
  result = api_instance.get_api_resources
  p result
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthenticationV1Api->get_api_resources: #{e}"
end
```

#### Using the get_api_resources_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<V1APIResourceList>, Integer, Hash)> get_api_resources_with_http_info

```ruby
begin
  
  data, status_code, headers = api_instance.get_api_resources_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <V1APIResourceList>
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthenticationV1Api->get_api_resources_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**V1APIResourceList**](V1APIResourceList.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf

