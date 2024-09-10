# Kubernetes::V2beta2ExternalMetricStatus

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **current** | [**V2beta2MetricValueStatus**](V2beta2MetricValueStatus.md) |  |  |
| **metric** | [**V2beta2MetricIdentifier**](V2beta2MetricIdentifier.md) |  |  |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V2beta2ExternalMetricStatus.new(
  current: null,
  metric: null
)
```

