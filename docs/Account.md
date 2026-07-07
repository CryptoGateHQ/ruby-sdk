# GriffNode::Account

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **plan** | [**AccountPlan**](AccountPlan.md) |  | [optional] |
| **usage** | [**AccountUsage**](AccountUsage.md) |  | [optional] |
| **limits** | [**AccountLimits**](AccountLimits.md) |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::Account.new(
  plan: null,
  usage: null,
  limits: null
)
```

