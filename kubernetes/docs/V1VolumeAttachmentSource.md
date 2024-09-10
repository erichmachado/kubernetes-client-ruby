# Kubernetes::V1VolumeAttachmentSource

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **persistent_volume_name** | **String** | Name of the persistent volume to attach. | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1VolumeAttachmentSource.new(
  persistent_volume_name: null
)
```

