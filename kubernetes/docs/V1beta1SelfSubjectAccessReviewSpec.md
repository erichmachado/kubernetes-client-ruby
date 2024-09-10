# Kubernetes::V1beta1SelfSubjectAccessReviewSpec

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **non_resource_attributes** | [**V1beta1NonResourceAttributes**](V1beta1NonResourceAttributes.md) |  | [optional] |
| **resource_attributes** | [**V1beta1ResourceAttributes**](V1beta1ResourceAttributes.md) |  | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1SelfSubjectAccessReviewSpec.new(
  non_resource_attributes: null,
  resource_attributes: null
)
```

