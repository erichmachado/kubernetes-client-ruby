# Kubernetes::V1beta1DeviceClaimConfiguration

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **opaque** | [**V1beta1OpaqueDeviceConfiguration**](V1beta1OpaqueDeviceConfiguration.md) |  | [optional] |
| **requests** | **Array&lt;String&gt;** | Requests lists the names of requests where the configuration applies. If empty, it applies to all requests. | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1DeviceClaimConfiguration.new(
  opaque: null,
  requests: null
)
```

