# GriffNode::InlineObject

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **success** | **Object** |  |  |
| **error** | **String** | Machine-readable code. |  |
| **message** | **String** | Human-readable description. |  |
| **existing_transaction** | [**InlineObjectAllOfExistingTransaction**](InlineObjectAllOfExistingTransaction.md) |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::InlineObject.new(
  success: null,
  error: null,
  message: null,
  existing_transaction: null
)
```

