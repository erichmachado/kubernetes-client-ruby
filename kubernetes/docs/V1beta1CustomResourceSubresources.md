# Kubernetes::V1beta1CustomResourceSubresources

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **scale** | [**V1beta1CustomResourceSubresourceScale**](V1beta1CustomResourceSubresourceScale.md) |  | [optional] |
| **status** | **Object** | Status denotes the status subresource for CustomResources | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1CustomResourceSubresources.new(
  scale: null,
  status: null
)
```

