# GriffNode::Transaction

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **transaction_id** | **String** |  |  |
| **status** | [**TransactionStatus**](TransactionStatus.md) |  |  |
| **type** | **String** |  | [optional] |
| **crypto** | [**CryptoSymbol**](CryptoSymbol.md) |  |  |
| **deposit_address** | **String** |  | [optional] |
| **amount_crypto** | **Float** |  | [optional] |
| **amount_fiat** | **Float** |  |  |
| **amount_usd** | **Float** |  |  |
| **amount_paid** | **Float** |  | [optional] |
| **amount_remaining** | **Float** |  | [optional] |
| **currency_fiat** | [**FiatCurrency**](FiatCurrency.md) |  | [default to &#39;USD&#39;] |
| **fiat_to_usd_rate** | **Float** |  | [optional] |
| **exchange_rate** | **Float** | USD per unit of crypto, locked at creation. | [optional] |
| **confirmations_required** | **Integer** |  | [optional] |
| **payment_url** | **String** |  | [optional] |
| **order_id** | **String** |  | [optional] |
| **customer_email** | **String** |  | [optional] |
| **items** | [**Array&lt;LineItem&gt;**](LineItem.md) |  | [optional] |
| **payments** | [**Array&lt;PaymentSplit&gt;**](PaymentSplit.md) | On-chain payments detected toward this transaction. | [optional] |
| **metadata** | **Hash&lt;String, String&gt;** | Free-form key/value (≤20 keys, string values ≤500 chars, ≤4 KB total). | [optional] |
| **success_url** | **String** |  | [optional] |
| **cancel_url** | **String** |  | [optional] |
| **created_at** | **Time** |  |  |
| **updated_at** | **Time** |  | [optional] |
| **expires_at** | **Time** |  |  |

## Example

```ruby
require 'griffnode'

instance = GriffNode::Transaction.new(
  transaction_id: null,
  status: null,
  type: null,
  crypto: null,
  deposit_address: null,
  amount_crypto: null,
  amount_fiat: null,
  amount_usd: null,
  amount_paid: null,
  amount_remaining: null,
  currency_fiat: null,
  fiat_to_usd_rate: null,
  exchange_rate: null,
  confirmations_required: null,
  payment_url: null,
  order_id: null,
  customer_email: null,
  items: null,
  payments: null,
  metadata: null,
  success_url: null,
  cancel_url: null,
  created_at: null,
  updated_at: null,
  expires_at: null
)
```

