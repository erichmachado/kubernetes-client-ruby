# Kubernetes::V1beta1StatefulSetUpdateStrategy

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **rolling_update** | [**V1beta1RollingUpdateStatefulSetStrategy**](V1beta1RollingUpdateStatefulSetStrategy.md) |  | [optional] |
| **type** | **String** | Type indicates the type of the StatefulSetUpdateStrategy. | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1StatefulSetUpdateStrategy.new(
  rolling_update: null,
  type: null
)
```

