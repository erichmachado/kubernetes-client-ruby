# Kubernetes::V1beta2ScaleSpec

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **replicas** | **Integer** | desired number of instances for the scaled object. | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta2ScaleSpec.new(
  replicas: null
)
```

