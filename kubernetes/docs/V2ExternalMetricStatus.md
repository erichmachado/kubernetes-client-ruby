# Kubernetes::V2ExternalMetricStatus

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **current** | [**V2MetricValueStatus**](V2MetricValueStatus.md) |  |  |
| **metric** | [**V2MetricIdentifier**](V2MetricIdentifier.md) |  |  |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V2ExternalMetricStatus.new(
  current: null,
  metric: null
)
```

