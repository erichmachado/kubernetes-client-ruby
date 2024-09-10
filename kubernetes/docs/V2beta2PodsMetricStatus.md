# Kubernetes::V2beta2PodsMetricStatus

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **current** | [**V2beta2MetricValueStatus**](V2beta2MetricValueStatus.md) |  |  |
| **metric** | [**V2beta2MetricIdentifier**](V2beta2MetricIdentifier.md) |  |  |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V2beta2PodsMetricStatus.new(
  current: null,
  metric: null
)
```

