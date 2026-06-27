# CryptoGate::AccountApi

All URIs are relative to *https://api.cryptogate.live/v1*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_account**](AccountApi.md#get_account) | **GET** /account | Merchant plan, usage and limits |
| [**get_stats**](AccountApi.md#get_stats) | **GET** /stats | Merchant transaction analytics |
| [**list_balances**](AccountApi.md#list_balances) | **GET** /balances | On-platform balances (for overage/top-up; NOT crypto settlement) |
| [**list_invoices**](AccountApi.md#list_invoices) | **GET** /invoices | CryptoGate billing invoices (platform ↔ merchant) |
| [**list_plans**](AccountApi.md#list_plans) | **GET** /plans | Plan catalogue and pricing |


## get_account

> <GetAccount200Response> get_account

Merchant plan, usage and limits

### Examples

```ruby
require 'time'
require 'cryptogate'
# setup authorization
CryptoGate.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = CryptoGate::AccountApi.new

begin
  # Merchant plan, usage and limits
  result = api_instance.get_account
  p result
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->get_account: #{e}"
end
```

#### Using the get_account_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GetAccount200Response>, Integer, Hash)> get_account_with_http_info

```ruby
begin
  # Merchant plan, usage and limits
  data, status_code, headers = api_instance.get_account_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GetAccount200Response>
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->get_account_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetAccount200Response**](GetAccount200Response.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_stats

> <GetStats200Response> get_stats

Merchant transaction analytics

### Examples

```ruby
require 'time'
require 'cryptogate'
# setup authorization
CryptoGate.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = CryptoGate::AccountApi.new

begin
  # Merchant transaction analytics
  result = api_instance.get_stats
  p result
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->get_stats: #{e}"
end
```

#### Using the get_stats_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GetStats200Response>, Integer, Hash)> get_stats_with_http_info

```ruby
begin
  # Merchant transaction analytics
  data, status_code, headers = api_instance.get_stats_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GetStats200Response>
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->get_stats_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetStats200Response**](GetStats200Response.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_balances

> <ListBalances200Response> list_balances

On-platform balances (for overage/top-up; NOT crypto settlement)

### Examples

```ruby
require 'time'
require 'cryptogate'
# setup authorization
CryptoGate.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = CryptoGate::AccountApi.new

begin
  # On-platform balances (for overage/top-up; NOT crypto settlement)
  result = api_instance.list_balances
  p result
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->list_balances: #{e}"
end
```

#### Using the list_balances_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ListBalances200Response>, Integer, Hash)> list_balances_with_http_info

```ruby
begin
  # On-platform balances (for overage/top-up; NOT crypto settlement)
  data, status_code, headers = api_instance.list_balances_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ListBalances200Response>
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->list_balances_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ListBalances200Response**](ListBalances200Response.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_invoices

> <ListInvoices200Response> list_invoices(opts)

CryptoGate billing invoices (platform ↔ merchant)

### Examples

```ruby
require 'time'
require 'cryptogate'
# setup authorization
CryptoGate.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = CryptoGate::AccountApi.new
opts = {
  limit: 56, # Integer | 
  offset: 56 # Integer | 
}

begin
  # CryptoGate billing invoices (platform ↔ merchant)
  result = api_instance.list_invoices(opts)
  p result
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->list_invoices: #{e}"
end
```

#### Using the list_invoices_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ListInvoices200Response>, Integer, Hash)> list_invoices_with_http_info(opts)

```ruby
begin
  # CryptoGate billing invoices (platform ↔ merchant)
  data, status_code, headers = api_instance.list_invoices_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ListInvoices200Response>
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->list_invoices_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **limit** | **Integer** |  | [optional][default to 20] |
| **offset** | **Integer** |  | [optional][default to 0] |

### Return type

[**ListInvoices200Response**](ListInvoices200Response.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_plans

> <ListPlans200Response> list_plans

Plan catalogue and pricing

### Examples

```ruby
require 'time'
require 'cryptogate'
# setup authorization
CryptoGate.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = CryptoGate::AccountApi.new

begin
  # Plan catalogue and pricing
  result = api_instance.list_plans
  p result
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->list_plans: #{e}"
end
```

#### Using the list_plans_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ListPlans200Response>, Integer, Hash)> list_plans_with_http_info

```ruby
begin
  # Plan catalogue and pricing
  data, status_code, headers = api_instance.list_plans_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ListPlans200Response>
rescue CryptoGate::ApiError => e
  puts "Error when calling AccountApi->list_plans_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ListPlans200Response**](ListPlans200Response.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

