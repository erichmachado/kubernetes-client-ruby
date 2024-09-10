# Kubernetes::V1ScaleSpec

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **replicas** | **Integer** | desired number of instances for the scaled object. | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1ScaleSpec.new(
  replicas: null
)
```

