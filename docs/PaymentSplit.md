# GriffNode::PaymentSplit

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **txid** | **String** | On-chain transaction hash (blockchain id, NOT the GriffNode transaction_id). | [optional] |
| **amount_crypto** | **Float** |  | [optional] |
| **confirmations** | **Integer** |  | [optional] |
| **status** | **String** |  | [optional] |
| **detected_at** | **Time** |  | [optional] |
| **confirmed_at** | **Time** |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::PaymentSplit.new(
  txid: null,
  amount_crypto: null,
  confirmations: null,
  status: null,
  detected_at: null,
  confirmed_at: null
)
```

