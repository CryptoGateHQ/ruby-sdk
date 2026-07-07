# GriffNode::DefaultApi

All URIs are relative to *https://api.griffnode.com/v1*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**payment_webhook**](DefaultApi.md#payment_webhook) | **POST** /paymentEvent | Payment lifecycle event delivered to the merchant&#39;s webhook URL |


## payment_webhook

> payment_webhook(opts)

Payment lifecycle event delivered to the merchant's webhook URL

Signed with HMAC-SHA256 over the RAW request body. Verify by comparing `X-GriffNode-Signature: sha256=<hex>` to `hex(hmac_sha256(webhook_secret, raw_body))` using a constant-time compare. Also sent: `X-GriffNode-Event` (the event type) and `X-Webhook-ID` (unique delivery id — use for idempotency). 

### Examples

```ruby
require 'time'
require 'griffnode'
# setup authorization
GriffNode.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = GriffNode::DefaultApi.new
opts = {
  webhook_payload:  # WebhookPayload | 
}

begin
  # Payment lifecycle event delivered to the merchant's webhook URL
  api_instance.payment_webhook(opts)
rescue GriffNode::ApiError => e
  puts "Error when calling DefaultApi->payment_webhook: #{e}"
end
```

#### Using the payment_webhook_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> payment_webhook_with_http_info(opts)

```ruby
begin
  # Payment lifecycle event delivered to the merchant's webhook URL
  data, status_code, headers = api_instance.payment_webhook_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue GriffNode::ApiError => e
  puts "Error when calling DefaultApi->payment_webhook_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **webhook_payload** | [**WebhookPayload**](WebhookPayload.md) |  | [optional] |

### Return type

nil (empty response body)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

