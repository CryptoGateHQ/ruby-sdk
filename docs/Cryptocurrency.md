# GriffNode::Cryptocurrency

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **symbol** | [**CryptoSymbol**](CryptoSymbol.md) |  | [optional] |
| **name** | **String** |  | [optional] |
| **blockchain** | **String** |  | [optional] |
| **network** | **String** |  | [optional] |
| **type** | **String** |  | [optional] |

## Example

```ruby
require 'griffnode'

instance = GriffNode::Cryptocurrency.new(
  symbol: null,
  name: null,
  blockchain: null,
  network: null,
  type: null
)
```

