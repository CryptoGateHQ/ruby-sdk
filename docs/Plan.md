# GriffNode::Plan

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tier** | [**PlanTier**](PlanTier.md) |  | [optional] |
| **monthly_price_usd** | **Float** |  | [optional] |
| **yearly_price_usd** | **Float** |  | [optional] |
| **monthly_transaction_limit** | **Integer** |  | [optional] |
| **overage_cost_per_tx** | **Float** |  | [optional] |
| **webhook_support** | **Boolean** |  | [optional] |
| **webhook_limit** | **Integer** |  | [optional] |
| **ip_whitelist** | **Boolean** |  | [optional] |
| **api_rate_limit_per_minute** | **Integer** |  | [optional] |
| **api_rate_limit_per_hour** | **Integer** |  | [optional] |
| **custom_pricing** | **Boolean** |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::Plan.new(
  tier: null,
  monthly_price_usd: null,
  yearly_price_usd: null,
  monthly_transaction_limit: null,
  overage_cost_per_tx: null,
  webhook_support: null,
  webhook_limit: null,
  ip_whitelist: null,
  api_rate_limit_per_minute: null,
  api_rate_limit_per_hour: null,
  custom_pricing: null
)
```

