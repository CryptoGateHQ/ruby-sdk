# CryptoGate::AccountPlan

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **tier** | [**PlanTier**](PlanTier.md) |  | [optional] |
| **billing_cycle** | **String** |  | [optional] |
| **auto_renewal** | **Boolean** |  | [optional] |
| **expires_at** | **Time** |  | [optional] |

## Example

```ruby
require 'cryptogate'

instance = CryptoGate::AccountPlan.new(
  tier: null,
  billing_cycle: null,
  auto_renewal: null,
  expires_at: null
)
```

