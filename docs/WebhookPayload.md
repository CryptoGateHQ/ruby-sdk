# CryptoGate::WebhookPayload

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **event** | **String** |  |  |
| **timestamp** | **Time** |  |  |
| **transaction_id** | **String** |  |  |
| **status** | [**TransactionStatus**](TransactionStatus.md) |  |  |
| **currency_crypto** | [**CryptoSymbol**](CryptoSymbol.md) |  | [optional] |
| **currency_fiat** | [**FiatCurrency**](FiatCurrency.md) |  | [optional][default to &#39;USD&#39;] |
| **amount_fiat** | **String** | Decimal string. | [optional] |
| **amount_usd** | **String** | Decimal string. | [optional] |
| **amount_crypto** | **String** | Decimal string. | [optional] |
| **order_id** | **String** |  | [optional] |
| **receipt_url** | **String** | Present on completed/overpaid. | [optional] |
| **metadata** | **Hash&lt;String, String&gt;** | Free-form key/value (≤20 keys, string values ≤500 chars, ≤4 KB total). | [optional] |

## Example

```ruby
require 'cryptogate'

instance = CryptoGate::WebhookPayload.new(
  event: null,
  timestamp: null,
  transaction_id: null,
  status: null,
  currency_crypto: null,
  currency_fiat: null,
  amount_fiat: null,
  amount_usd: null,
  amount_crypto: null,
  order_id: null,
  receipt_url: null,
  metadata: null
)
```

