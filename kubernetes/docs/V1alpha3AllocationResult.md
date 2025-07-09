# Kubernetes::V1alpha3AllocationResult

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **devices** | [**V1alpha3DeviceAllocationResult**](V1alpha3DeviceAllocationResult.md) |  | [optional] |
| **node_selector** | [**V1NodeSelector**](V1NodeSelector.md) |  | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1alpha3AllocationResult.new(
  devices: null,
  node_selector: null
)
```

