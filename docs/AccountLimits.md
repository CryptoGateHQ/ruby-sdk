# GriffNode::AccountLimits

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **api_rate_limit_per_minute** | **Integer** |  | [optional] |
| **api_rate_limit_per_hour** | **Integer** |  | [optional] |
| **webhook_support** | **Boolean** |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::AccountLimits.new(
  api_rate_limit_per_minute: null,
  api_rate_limit_per_hour: null,
  webhook_support: null
)
```

