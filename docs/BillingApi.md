# GriffNode::BillingApi

All URIs are relative to *https://api.griffnode.com/v1*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_billing_checkout**](BillingApi.md#create_billing_checkout) | **POST** /billing/checkout | Start a plan upgrade or account top-up |


## create_billing_checkout

> <TransactionEnvelope> create_billing_checkout(create_billing_checkout_request)

Start a plan upgrade or account top-up

### Examples

```ruby
require 'time'
require 'griffnode'
# setup authorization
GriffNode.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = GriffNode::BillingApi.new
create_billing_checkout_request = GriffNode::CreateBillingCheckoutRequest.new({tier: GriffNode::PlanTier::STARTER}) # CreateBillingCheckoutRequest | 

begin
  # Start a plan upgrade or account top-up
  result = api_instance.create_billing_checkout(create_billing_checkout_request)
  p result
rescue GriffNode::ApiError => e
  puts "Error when calling BillingApi->create_billing_checkout: #{e}"
end
```

#### Using the create_billing_checkout_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionEnvelope>, Integer, Hash)> create_billing_checkout_with_http_info(create_billing_checkout_request)

```ruby
begin
  # Start a plan upgrade or account top-up
  data, status_code, headers = api_instance.create_billing_checkout_with_http_info(create_billing_checkout_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionEnvelope>
rescue GriffNode::ApiError => e
  puts "Error when calling BillingApi->create_billing_checkout_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **create_billing_checkout_request** | [**CreateBillingCheckoutRequest**](CreateBillingCheckoutRequest.md) |  |  |

### Return type

[**TransactionEnvelope**](TransactionEnvelope.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

