# GriffNode::Balance

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **currency** | **String** |  | [optional] |
| **available_balance** | **Float** |  | [optional] |
| **pending_balance** | **Float** |  | [optional] |
| **updated_at** | **Time** |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::Balance.new(
  currency: null,
  available_balance: null,
  pending_balance: null,
  updated_at: null
)
```

