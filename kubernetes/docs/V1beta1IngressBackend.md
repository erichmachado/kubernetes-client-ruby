# Kubernetes::V1beta1IngressBackend

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **service_name** | **String** | Specifies the name of the referenced service. |  |
| **service_port** | **Object** | Specifies the port of the referenced service. |  |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1IngressBackend.new(
  service_name: null,
  service_port: null
)
```

