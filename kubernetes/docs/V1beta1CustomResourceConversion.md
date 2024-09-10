# Kubernetes::V1beta1CustomResourceConversion

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **strategy** | **String** | &#x60;strategy&#x60; specifies the conversion strategy. Allowed values are: - &#x60;None&#x60;: The converter only change the apiVersion and would not touch any other field in the CR. - &#x60;Webhook&#x60;: API Server will call to an external webhook to do the conversion. Additional information is needed for this option. |  |
| **webhook_client_config** | [**ApiextensionsV1beta1WebhookClientConfig**](ApiextensionsV1beta1WebhookClientConfig.md) |  | [optional] |

## Example

```ruby
require 'kubernetes-io'

instance = Kubernetes::V1beta1CustomResourceConversion.new(
  strategy: null,
  webhook_client_config: null
)
```

