# Kubernetes::V1beta1AllocationResult

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **devices** | [**V1beta1DeviceAllocationResult**](V1beta1DeviceAllocationResult.md) |  | [optional] |
| **node_selector** | [**V1NodeSelector**](V1NodeSelector.md) |  | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1AllocationResult.new(
  devices: null,
  node_selector: null
)
```

