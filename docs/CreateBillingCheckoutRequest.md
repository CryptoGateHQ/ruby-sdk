# GriffNode::CreateBillingCheckoutRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tier** | [**PlanTier**](PlanTier.md) |  |  |
| **billing_months** | **Integer** |  | [optional][default to 1] |
| **payment_method** | **String** |  | [optional][default to &#39;crypto&#39;] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::CreateBillingCheckoutRequest.new(
  tier: null,
  billing_months: null,
  payment_method: null
)
```

