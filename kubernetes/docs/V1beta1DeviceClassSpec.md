# Kubernetes::V1beta1DeviceClassSpec

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **config** | [**Array&lt;V1beta1DeviceClassConfiguration&gt;**](V1beta1DeviceClassConfiguration.md) | Config defines configuration parameters that apply to each device that is claimed via this class. Some classses may potentially be satisfied by multiple drivers, so each instance of a vendor configuration applies to exactly one driver.  They are passed to the driver, but are not considered while allocating the claim. | [optional] |
| **selectors** | [**Array&lt;V1beta1DeviceSelector&gt;**](V1beta1DeviceSelector.md) | Each selector must be satisfied by a device which is claimed via this class. | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1DeviceClassSpec.new(
  config: null,
  selectors: null
)
```

