# Kubernetes::V1LocalObjectReference

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **name** | **String** | Name of the referent. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1LocalObjectReference.new(
  name: null
)
```

