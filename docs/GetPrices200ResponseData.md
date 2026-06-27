# CryptoGate::GetPrices200ResponseData

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **crypto** | **Hash&lt;String, Float&gt;** | USD price per unit, keyed by crypto symbol (active coins only). | [optional] |
| **fiat** | **Hash&lt;String, Float&gt;** | USD value of one unit of each fiat currency. | [optional] |
| **fetched_at** | **Time** |  | [optional] |

## Example

```ruby
require 'cryptogate'

instance = CryptoGate::GetPrices200ResponseData.new(
  crypto: null,
  fiat: null,
  fetched_at: null
)
```

