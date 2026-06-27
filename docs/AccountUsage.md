# CryptoGate::AccountUsage

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **monthly_transactions_used** | **Integer** |  | [optional] |
| **monthly_transaction_limit** | **Integer** | null &#x3D; unlimited. | [optional] |
| **overage_cost_per_tx** | **Float** |  | [optional] |

## Example

```ruby
require 'cryptogate'

instance = CryptoGate::AccountUsage.new(
  monthly_transactions_used: null,
  monthly_transaction_limit: null,
  overage_cost_per_tx: null
)
```

