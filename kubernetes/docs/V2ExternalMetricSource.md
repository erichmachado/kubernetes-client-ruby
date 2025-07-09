# Kubernetes::V2ExternalMetricSource

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **metric** | [**V2MetricIdentifier**](V2MetricIdentifier.md) |  |  |
| **target** | [**V2MetricTarget**](V2MetricTarget.md) |  |  |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V2ExternalMetricSource.new(
  metric: null,
  target: null
)
```

