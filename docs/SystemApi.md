# GriffNode::SystemApi

All URIs are relative to *https://api.griffnode.com/v1*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_health**](SystemApi.md#get_health) | **GET** /health | API health check |
| [**hosted_checkout_redirect**](SystemApi.md#hosted_checkout_redirect) | **GET** /pay | Hosted-checkout redirect (browser flow, publishable key) |


## get_health

> <GetHealth200Response> get_health

API health check

### Examples

```ruby
require 'time'
require 'griffnode'

api_instance = GriffNode::SystemApi.new

begin
  # API health check
  result = api_instance.get_health
  p result
rescue GriffNode::ApiError => e
  puts "Error when calling SystemApi->get_health: #{e}"
end
```

#### Using the get_health_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GetHealth200Response>, Integer, Hash)> get_health_with_http_info

```ruby
begin
  # API health check
  data, status_code, headers = api_instance.get_health_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GetHealth200Response>
rescue GriffNode::ApiError => e
  puts "Error when calling SystemApi->get_health_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetHealth200Response**](GetHealth200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## hosted_checkout_redirect

> hosted_checkout_redirect(pk, amount, crypto, opts)

Hosted-checkout redirect (browser flow, publishable key)

Browser-facing redirect to the hosted payment page, authenticated by a **publishable** key in the query string (safe to expose client-side). Not used by the server-side SDKs — included for completeness. 

### Examples

```ruby
require 'time'
require 'griffnode'

api_instance = GriffNode::SystemApi.new
pk = 'pk_example' # String | Publishable key, pk_live_… / pk_test_…
amount = 'amount_example' # String | Fiat amount (≥ 1.00 USD equivalent).
crypto = GriffNode::CryptoSymbol::BTC # CryptoSymbol | 
opts = {
  link: 'link_example' # String | Payment-link slug for attribution.
}

begin
  # Hosted-checkout redirect (browser flow, publishable key)
  api_instance.hosted_checkout_redirect(pk, amount, crypto, opts)
rescue GriffNode::ApiError => e
  puts "Error when calling SystemApi->hosted_checkout_redirect: #{e}"
end
```

#### Using the hosted_checkout_redirect_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> hosted_checkout_redirect_with_http_info(pk, amount, crypto, opts)

```ruby
begin
  # Hosted-checkout redirect (browser flow, publishable key)
  data, status_code, headers = api_instance.hosted_checkout_redirect_with_http_info(pk, amount, crypto, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue GriffNode::ApiError => e
  puts "Error when calling SystemApi->hosted_checkout_redirect_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **pk** | **String** | Publishable key, pk_live_… / pk_test_… |  |
| **amount** | **String** | Fiat amount (≥ 1.00 USD equivalent). |  |
| **crypto** | [**CryptoSymbol**](.md) |  |  |
| **link** | **String** | Payment-link slug for attribution. | [optional] |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

