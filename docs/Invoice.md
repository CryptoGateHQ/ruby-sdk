# GriffNode::Invoice

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **transaction_id** | **String** |  | [optional] |
| **purchase_type** | **String** |  | [optional] |
| **amount_fiat** | **Float** |  | [optional] |
| **currency_fiat** | [**FiatCurrency**](FiatCurrency.md) |  | [optional][default to &#39;USD&#39;] |
| **status** | **String** |  | [optional] |
| **crypto_symbol** | [**CryptoSymbol**](CryptoSymbol.md) |  | [optional] |
| **created_at** | **Time** |  | [optional] |
| **confirmed_at** | **Time** |  | [optional] |
| **expires_at** | **Time** |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::Invoice.new(
  transaction_id: null,
  purchase_type: null,
  amount_fiat: null,
  currency_fiat: null,
  status: null,
  crypto_symbol: null,
  created_at: null,
  confirmed_at: null,
  expires_at: null
)
```

