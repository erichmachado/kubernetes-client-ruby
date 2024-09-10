# Kubernetes::V1beta1EventSeries

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **count** | **Integer** | Number of occurrences in this series up to the last heartbeat time |  |
| **last_observed_time** | **Time** | Time when last Event from the series was seen before last heartbeat. |  |
| **state** | **String** | Information whether this series is ongoing or finished. |  |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1EventSeries.new(
  count: null,
  last_observed_time: null,
  state: null
)
```

