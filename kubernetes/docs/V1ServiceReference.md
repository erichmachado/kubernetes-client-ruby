# Kubernetes::V1ServiceReference

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** | Name is the name of the service | [optional] |
| **namespace** | **String** | Namespace is the namespace of the service | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1ServiceReference.new(
  name: null,
  namespace: null
)
```

