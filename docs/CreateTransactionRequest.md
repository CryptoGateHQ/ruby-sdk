# GriffNode::CreateTransactionRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **crypto** | [**CryptoSymbol**](CryptoSymbol.md) |  |  |
| **amount** | **Float** | Fiat amount (≥ 1.00 USD equivalent). |  |
| **currency_fiat** | [**FiatCurrency**](FiatCurrency.md) |  | [optional][default to &#39;USD&#39;] |
| **metadata** | **Hash&lt;String, String&gt;** | Free-form key/value (≤20 keys, string values ≤500 chars, ≤4 KB total). | [optional] |
| **customer_email** | **String** |  | [optional] |
| **success_url** | **String** |  | [optional] |
| **cancel_url** | **String** |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::CreateTransactionRequest.new(
  crypto: null,
  amount: null,
  currency_fiat: null,
  metadata: null,
  customer_email: null,
  success_url: null,
  cancel_url: null
)
```

