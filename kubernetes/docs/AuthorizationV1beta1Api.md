# Kubernetes::AuthorizationV1beta1Api

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_namespaced_local_subject_access_review**](AuthorizationV1beta1Api.md#create_namespaced_local_subject_access_review) | **POST** /apis/authorization.k8s.io/v1beta1/namespaces/{namespace}/localsubjectaccessreviews |  |
| [**create_self_subject_access_review**](AuthorizationV1beta1Api.md#create_self_subject_access_review) | **POST** /apis/authorization.k8s.io/v1beta1/selfsubjectaccessreviews |  |
| [**create_self_subject_rules_review**](AuthorizationV1beta1Api.md#create_self_subject_rules_review) | **POST** /apis/authorization.k8s.io/v1beta1/selfsubjectrulesreviews |  |
| [**create_subject_access_review**](AuthorizationV1beta1Api.md#create_subject_access_review) | **POST** /apis/authorization.k8s.io/v1beta1/subjectaccessreviews |  |
| [**get_api_resources**](AuthorizationV1beta1Api.md#get_api_resources) | **GET** /apis/authorization.k8s.io/v1beta1/ |  |


## create_namespaced_local_subject_access_review

> <V1beta1LocalSubjectAccessReview> create_namespaced_local_subject_access_review(namespace, body, opts)



create a LocalSubjectAccessReview

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

api_instance = Kubernetes::AuthorizationV1beta1Api.new
namespace = 'namespace_example' # String | object name and auth scope, such as for teams and projects
body = Kubernetes::V1beta1LocalSubjectAccessReview.new({spec: Kubernetes::V1beta1SubjectAccessReviewSpec.new}) # V1beta1LocalSubjectAccessReview | 
opts = {
  dry_run: 'dry_run_example', # String | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed
  include_uninitialized: true, # Boolean | If IncludeUninitialized is specified, the object may be returned without completing initialization.
  pretty: 'pretty_example' # String | If 'true', then the output is pretty printed.
}

begin
  
  result = api_instance.create_namespaced_local_subject_access_review(namespace, body, opts)
  p result
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthorizationV1beta1Api->create_namespaced_local_subject_access_review: #{e}"
end
```

#### Using the create_namespaced_local_subject_access_review_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<V1beta1LocalSubjectAccessReview>, Integer, Hash)> create_namespaced_local_subject_access_review_with_http_info(namespace, body, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.create_namespaced_local_subject_access_review_with_http_info(namespace, body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <V1beta1LocalSubjectAccessReview>
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthorizationV1beta1Api->create_namespaced_local_subject_access_review_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **namespace** | **String** | object name and auth scope, such as for teams and projects |  |
| **body** | [**V1beta1LocalSubjectAccessReview**](V1beta1LocalSubjectAccessReview.md) |  |  |
| **dry_run** | **String** | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] |
| **include_uninitialized** | **Boolean** | If IncludeUninitialized is specified, the object may be returned without completing initialization. | [optional] |
| **pretty** | **String** | If &#39;true&#39;, then the output is pretty printed. | [optional] |

### Return type

[**V1beta1LocalSubjectAccessReview**](V1beta1LocalSubjectAccessReview.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf


## create_self_subject_access_review

> <V1beta1SelfSubjectAccessReview> create_self_subject_access_review(body, opts)



create a SelfSubjectAccessReview

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

api_instance = Kubernetes::AuthorizationV1beta1Api.new
body = Kubernetes::V1beta1SelfSubjectAccessReview.new({spec: Kubernetes::V1beta1SelfSubjectAccessReviewSpec.new}) # V1beta1SelfSubjectAccessReview | 
opts = {
  dry_run: 'dry_run_example', # String | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed
  include_uninitialized: true, # Boolean | If IncludeUninitialized is specified, the object may be returned without completing initialization.
  pretty: 'pretty_example' # String | If 'true', then the output is pretty printed.
}

begin
  
  result = api_instance.create_self_subject_access_review(body, opts)
  p result
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthorizationV1beta1Api->create_self_subject_access_review: #{e}"
end
```

#### Using the create_self_subject_access_review_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<V1beta1SelfSubjectAccessReview>, Integer, Hash)> create_self_subject_access_review_with_http_info(body, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.create_self_subject_access_review_with_http_info(body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <V1beta1SelfSubjectAccessReview>
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthorizationV1beta1Api->create_self_subject_access_review_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **body** | [**V1beta1SelfSubjectAccessReview**](V1beta1SelfSubjectAccessReview.md) |  |  |
| **dry_run** | **String** | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] |
| **include_uninitialized** | **Boolean** | If IncludeUninitialized is specified, the object may be returned without completing initialization. | [optional] |
| **pretty** | **String** | If &#39;true&#39;, then the output is pretty printed. | [optional] |

### Return type

[**V1beta1SelfSubjectAccessReview**](V1beta1SelfSubjectAccessReview.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf


## create_self_subject_rules_review

> <V1beta1SelfSubjectRulesReview> create_self_subject_rules_review(body, opts)



create a SelfSubjectRulesReview

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

api_instance = Kubernetes::AuthorizationV1beta1Api.new
body = Kubernetes::V1beta1SelfSubjectRulesReview.new({spec: Kubernetes::V1beta1SelfSubjectRulesReviewSpec.new}) # V1beta1SelfSubjectRulesReview | 
opts = {
  dry_run: 'dry_run_example', # String | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed
  include_uninitialized: true, # Boolean | If IncludeUninitialized is specified, the object may be returned without completing initialization.
  pretty: 'pretty_example' # String | If 'true', then the output is pretty printed.
}

begin
  
  result = api_instance.create_self_subject_rules_review(body, opts)
  p result
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthorizationV1beta1Api->create_self_subject_rules_review: #{e}"
end
```

#### Using the create_self_subject_rules_review_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<V1beta1SelfSubjectRulesReview>, Integer, Hash)> create_self_subject_rules_review_with_http_info(body, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.create_self_subject_rules_review_with_http_info(body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <V1beta1SelfSubjectRulesReview>
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthorizationV1beta1Api->create_self_subject_rules_review_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **body** | [**V1beta1SelfSubjectRulesReview**](V1beta1SelfSubjectRulesReview.md) |  |  |
| **dry_run** | **String** | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] |
| **include_uninitialized** | **Boolean** | If IncludeUninitialized is specified, the object may be returned without completing initialization. | [optional] |
| **pretty** | **String** | If &#39;true&#39;, then the output is pretty printed. | [optional] |

### Return type

[**V1beta1SelfSubjectRulesReview**](V1beta1SelfSubjectRulesReview.md)

### Authorization

[BearerToken](../README.md#BearerToken)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, application/yaml, application/vnd.kubernetes.protobuf


## create_subject_access_review

> <V1beta1SubjectAccessReview> create_subject_access_review(body, opts)



create a SubjectAccessReview

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

api_instance = Kubernetes::AuthorizationV1beta1Api.new
body = Kubernetes::V1beta1SubjectAccessReview.new({spec: Kubernetes::V1beta1SubjectAccessReviewSpec.new}) # V1beta1SubjectAccessReview | 
opts = {
  dry_run: 'dry_run_example', # String | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed
  include_uninitialized: true, # Boolean | If IncludeUninitialized is specified, the object may be returned without completing initialization.
  pretty: 'pretty_example' # String | If 'true', then the output is pretty printed.
}

begin
  
  result = api_instance.create_subject_access_review(body, opts)
  p result
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthorizationV1beta1Api->create_subject_access_review: #{e}"
end
```

#### Using the create_subject_access_review_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<V1beta1SubjectAccessReview>, Integer, Hash)> create_subject_access_review_with_http_info(body, opts)

```ruby
begin
  
  data, status_code, headers = api_instance.create_subject_access_review_with_http_info(body, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <V1beta1SubjectAccessReview>
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthorizationV1beta1Api->create_subject_access_review_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **body** | [**V1beta1SubjectAccessReview**](V1beta1SubjectAccessReview.md) |  |  |
| **dry_run** | **String** | When present, indicates that modifications should not be persisted. An invalid or unrecognized dryRun directive will result in an error response and no further processing of the request. Valid values are: - All: all dry run stages will be processed | [optional] |
| **include_uninitialized** | **Boolean** | If IncludeUninitialized is specified, the object may be returned without completing initialization. | [optional] |
| **pretty** | **String** | If &#39;true&#39;, then the output is pretty printed. | [optional] |

### Return type

[**V1beta1SubjectAccessReview**](V1beta1SubjectAccessReview.md)

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

api_instance = Kubernetes::AuthorizationV1beta1Api.new

begin
  
  result = api_instance.get_api_resources
  p result
rescue Kubernetes::ApiError => e
  puts "Error when calling AuthorizationV1beta1Api->get_api_resources: #{e}"
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
  puts "Error when calling AuthorizationV1beta1Api->get_api_resources_with_http_info: #{e}"
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

