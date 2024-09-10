# Kubernetes::V1VolumeError

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **message** | **String** | String detailing the error encountered during Attach or Detach operation. This string maybe logged, so it should not contain sensitive information. | [optional] |
| **time** | **Time** | Time the error was encountered. | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1VolumeError.new(
  message: null,
  time: null
)
```

