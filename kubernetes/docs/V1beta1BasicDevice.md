# Kubernetes::V1beta1BasicDevice

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **attributes** | [**Hash&lt;String, V1beta1DeviceAttribute&gt;**](V1beta1DeviceAttribute.md) | Attributes defines the set of attributes for this device. The name of each attribute must be unique in that set.  The maximum number of attributes and capacities combined is 32. | [optional] |
| **capacity** | [**Hash&lt;String, V1beta1DeviceCapacity&gt;**](V1beta1DeviceCapacity.md) | Capacity defines the set of capacities for this device. The name of each capacity must be unique in that set.  The maximum number of attributes and capacities combined is 32. | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1BasicDevice.new(
  attributes: null,
  capacity: null
)
```

