# GriffNode::MarketDataApi

All URIs are relative to *https://api.griffnode.com/v1*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_prices**](MarketDataApi.md#get_prices) | **GET** /prices | Current crypto and fiat exchange rates (USD-denominated) |
| [**list_cryptocurrencies**](MarketDataApi.md#list_cryptocurrencies) | **GET** /cryptos/list | All supported cryptocurrencies and tokens |
| [**list_merchant_cryptocurrencies**](MarketDataApi.md#list_merchant_cryptocurrencies) | **GET** /merchant/cryptos | Cryptocurrencies this merchant has wallets configured for |


## get_prices

> <GetPrices200Response> get_prices

Current crypto and fiat exchange rates (USD-denominated)

### Examples

```ruby
require 'time'
require 'griffnode'
# setup authorization
GriffNode.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = GriffNode::MarketDataApi.new

begin
  # Current crypto and fiat exchange rates (USD-denominated)
  result = api_instance.get_prices
  p result
rescue GriffNode::ApiError => e
  puts "Error when calling MarketDataApi->get_prices: #{e}"
end
```

#### Using the get_prices_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GetPrices200Response>, Integer, Hash)> get_prices_with_http_info

```ruby
begin
  # Current crypto and fiat exchange rates (USD-denominated)
  data, status_code, headers = api_instance.get_prices_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GetPrices200Response>
rescue GriffNode::ApiError => e
  puts "Error when calling MarketDataApi->get_prices_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetPrices200Response**](GetPrices200Response.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_cryptocurrencies

> <ListCryptocurrencies200Response> list_cryptocurrencies

All supported cryptocurrencies and tokens

### Examples

```ruby
require 'time'
require 'griffnode'
# setup authorization
GriffNode.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = GriffNode::MarketDataApi.new

begin
  # All supported cryptocurrencies and tokens
  result = api_instance.list_cryptocurrencies
  p result
rescue GriffNode::ApiError => e
  puts "Error when calling MarketDataApi->list_cryptocurrencies: #{e}"
end
```

#### Using the list_cryptocurrencies_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ListCryptocurrencies200Response>, Integer, Hash)> list_cryptocurrencies_with_http_info

```ruby
begin
  # All supported cryptocurrencies and tokens
  data, status_code, headers = api_instance.list_cryptocurrencies_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ListCryptocurrencies200Response>
rescue GriffNode::ApiError => e
  puts "Error when calling MarketDataApi->list_cryptocurrencies_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ListCryptocurrencies200Response**](ListCryptocurrencies200Response.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_merchant_cryptocurrencies

> <ListCryptocurrencies200Response> list_merchant_cryptocurrencies

Cryptocurrencies this merchant has wallets configured for

### Examples

```ruby
require 'time'
require 'griffnode'
# setup authorization
GriffNode.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = GriffNode::MarketDataApi.new

begin
  # Cryptocurrencies this merchant has wallets configured for
  result = api_instance.list_merchant_cryptocurrencies
  p result
rescue GriffNode::ApiError => e
  puts "Error when calling MarketDataApi->list_merchant_cryptocurrencies: #{e}"
end
```

#### Using the list_merchant_cryptocurrencies_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ListCryptocurrencies200Response>, Integer, Hash)> list_merchant_cryptocurrencies_with_http_info

```ruby
begin
  # Cryptocurrencies this merchant has wallets configured for
  data, status_code, headers = api_instance.list_merchant_cryptocurrencies_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ListCryptocurrencies200Response>
rescue GriffNode::ApiError => e
  puts "Error when calling MarketDataApi->list_merchant_cryptocurrencies_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ListCryptocurrencies200Response**](ListCryptocurrencies200Response.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

