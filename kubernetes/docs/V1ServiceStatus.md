# Kubernetes::V1ServiceStatus

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **load_balancer** | [**V1LoadBalancerStatus**](V1LoadBalancerStatus.md) |  | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1ServiceStatus.new(
  load_balancer: null
)
```

