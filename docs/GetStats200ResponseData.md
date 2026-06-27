# CryptoGate::GetStats200ResponseData

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **total_transactions** | **Integer** |  | [optional] |
| **monthly_transactions** | **Integer** |  | [optional] |
| **total_volume_fiat** | **Float** |  | [optional] |
| **unique_customers** | **Integer** |  | [optional] |

## Example

```ruby
require 'cryptogate'

instance = CryptoGate::GetStats200ResponseData.new(
  total_transactions: null,
  monthly_transactions: null,
  total_volume_fiat: null,
  unique_customers: null
)
```

