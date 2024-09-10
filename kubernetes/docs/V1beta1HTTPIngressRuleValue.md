# Kubernetes::V1beta1HTTPIngressRuleValue

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **paths** | [**Array&lt;V1beta1HTTPIngressPath&gt;**](V1beta1HTTPIngressPath.md) | A collection of paths that map requests to backends. |  |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1HTTPIngressRuleValue.new(
  paths: null
)
```

