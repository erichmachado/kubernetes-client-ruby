# Kubernetes::V1beta1LeaseSpec

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **acquire_time** | **Time** | acquireTime is a time when the current lease was acquired. | [optional] |
| **holder_identity** | **String** | holderIdentity contains the identity of the holder of a current lease. | [optional] |
| **lease_duration_seconds** | **Integer** | leaseDurationSeconds is a duration that candidates for a lease need to wait to force acquire it. This is measure against time of last observed RenewTime. | [optional] |
| **lease_transitions** | **Integer** | leaseTransitions is the number of transitions of a lease between holders. | [optional] |
| **renew_time** | **Time** | renewTime is a time when the current holder of a lease has last updated the lease. | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1LeaseSpec.new(
  acquire_time: null,
  holder_identity: null,
  lease_duration_seconds: null,
  lease_transitions: null,
  renew_time: null
)
```

