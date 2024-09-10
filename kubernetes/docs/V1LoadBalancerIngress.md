# Kubernetes::V1LoadBalancerIngress

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **hostname** | **String** | Hostname is set for load-balancer ingress points that are DNS based (typically AWS load-balancers) | [optional] |
| **ip** | **String** | IP is set for load-balancer ingress points that are IP based (typically GCE or OpenStack load-balancers) | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1LoadBalancerIngress.new(
  hostname: null,
  ip: null
)
```

