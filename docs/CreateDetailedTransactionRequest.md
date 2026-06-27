# CryptoGate::CreateDetailedTransactionRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **crypto** | [**CryptoSymbol**](CryptoSymbol.md) |  |  |
| **currency_fiat** | [**FiatCurrency**](FiatCurrency.md) |  | [optional][default to &#39;USD&#39;] |
| **items** | [**Array&lt;LineItem&gt;**](LineItem.md) |  |  |
| **order_id** | **String** |  |  |
| **metadata** | **Hash&lt;String, String&gt;** | Free-form key/value (≤20 keys, string values ≤500 chars, ≤4 KB total). | [optional] |
| **customer_email** | **String** |  | [optional] |
| **success_url** | **String** |  | [optional] |
| **cancel_url** | **String** |  | [optional] |

## Example

```ruby
require 'cryptogate'

instance = CryptoGate::CreateDetailedTransactionRequest.new(
  crypto: null,
  currency_fiat: null,
  items: null,
  order_id: null,
  metadata: null,
  customer_email: null,
  success_url: null,
  cancel_url: null
)
```

