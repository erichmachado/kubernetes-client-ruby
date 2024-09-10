# Kubernetes::V2beta2ResourceMetricStatus

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **current** | [**V2beta2MetricValueStatus**](V2beta2MetricValueStatus.md) |  |  |
| **name** | **String** | Name is the name of the resource in question. |  |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V2beta2ResourceMetricStatus.new(
  current: null,
  name: null
)
```

