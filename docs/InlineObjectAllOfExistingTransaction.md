# GriffNode::InlineObjectAllOfExistingTransaction

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **transaction_id** | **String** |  | [optional] |
| **status** | [**TransactionStatus**](TransactionStatus.md) |  | [optional] |
| **payment_url** | **String** |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::InlineObjectAllOfExistingTransaction.new(
  transaction_id: null,
  status: null,
  payment_url: null
)
```

