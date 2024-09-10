# Kubernetes::V1beta1CertificateSigningRequestCondition

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **last_update_time** | **Time** | timestamp for the last update to this condition | [optional] |
| **message** | **String** | human readable message with details about the request state | [optional] |
| **reason** | **String** | brief reason for the request state | [optional] |
| **type** | **String** | request approval state, currently Approved or Denied. |  |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1CertificateSigningRequestCondition.new(
  last_update_time: null,
  message: null,
  reason: null,
  type: null
)
```

