# GriffNode::Error

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **success** | **Object** |  |  |
| **error** | **String** | Machine-readable code. |  |
| **message** | **String** | Human-readable description. |  |

## Example

```ruby
require 'griffnode'

instance = GriffNode::Error.new(
  success: null,
  error: null,
  message: null
)
```

