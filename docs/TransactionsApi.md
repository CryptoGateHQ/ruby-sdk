# CryptoGate::TransactionsApi

All URIs are relative to *https://api.cryptogate.live/v1*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_detailed_transaction**](TransactionsApi.md#create_detailed_transaction) | **POST** /transactions/create-detailed | Create an itemized transaction (Professional/Enterprise plans) |
| [**create_transaction**](TransactionsApi.md#create_transaction) | **POST** /transactions/create | Create a payment transaction |
| [**get_transaction**](TransactionsApi.md#get_transaction) | **GET** /transactions/{transaction_id} | Retrieve a single transaction |
| [**list_transactions**](TransactionsApi.md#list_transactions) | **GET** /transactions/list | List the merchant&#39;s transactions (newest first) |


## create_detailed_transaction

> <TransactionEnvelope> create_detailed_transaction(create_detailed_transaction_request, opts)

Create an itemized transaction (Professional/Enterprise plans)

### Examples

```ruby
require 'time'
require 'cryptogate'
# setup authorization
CryptoGate.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = CryptoGate::TransactionsApi.new
create_detailed_transaction_request = CryptoGate::CreateDetailedTransactionRequest.new({crypto: CryptoGate::CryptoSymbol::BTC, items: [CryptoGate::LineItem.new({name: 'name_example', price: 3.56})], order_id: 'order_id_example'}) # CreateDetailedTransactionRequest | 
opts = {
  x_idempotency_key: 'x_idempotency_key_example' # String | Optional unique key for a create request (e.g. a UUID). A retried create with the same key returns the original transaction instead of creating a duplicate — send it on every create so a network retry can't double-charge the customer. 
}

begin
  # Create an itemized transaction (Professional/Enterprise plans)
  result = api_instance.create_detailed_transaction(create_detailed_transaction_request, opts)
  p result
rescue CryptoGate::ApiError => e
  puts "Error when calling TransactionsApi->create_detailed_transaction: #{e}"
end
```

#### Using the create_detailed_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionEnvelope>, Integer, Hash)> create_detailed_transaction_with_http_info(create_detailed_transaction_request, opts)

```ruby
begin
  # Create an itemized transaction (Professional/Enterprise plans)
  data, status_code, headers = api_instance.create_detailed_transaction_with_http_info(create_detailed_transaction_request, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionEnvelope>
rescue CryptoGate::ApiError => e
  puts "Error when calling TransactionsApi->create_detailed_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **create_detailed_transaction_request** | [**CreateDetailedTransactionRequest**](CreateDetailedTransactionRequest.md) |  |  |
| **x_idempotency_key** | **String** | Optional unique key for a create request (e.g. a UUID). A retried create with the same key returns the original transaction instead of creating a duplicate — send it on every create so a network retry can&#39;t double-charge the customer.  | [optional] |

### Return type

[**TransactionEnvelope**](TransactionEnvelope.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## create_transaction

> <TransactionEnvelope> create_transaction(create_transaction_request, opts)

Create a payment transaction

### Examples

```ruby
require 'time'
require 'cryptogate'
# setup authorization
CryptoGate.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = CryptoGate::TransactionsApi.new
create_transaction_request = CryptoGate::CreateTransactionRequest.new({crypto: CryptoGate::CryptoSymbol::BTC, amount: 3.56}) # CreateTransactionRequest | 
opts = {
  x_idempotency_key: 'x_idempotency_key_example' # String | Optional unique key for a create request (e.g. a UUID). A retried create with the same key returns the original transaction instead of creating a duplicate — send it on every create so a network retry can't double-charge the customer. 
}

begin
  # Create a payment transaction
  result = api_instance.create_transaction(create_transaction_request, opts)
  p result
rescue CryptoGate::ApiError => e
  puts "Error when calling TransactionsApi->create_transaction: #{e}"
end
```

#### Using the create_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionEnvelope>, Integer, Hash)> create_transaction_with_http_info(create_transaction_request, opts)

```ruby
begin
  # Create a payment transaction
  data, status_code, headers = api_instance.create_transaction_with_http_info(create_transaction_request, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionEnvelope>
rescue CryptoGate::ApiError => e
  puts "Error when calling TransactionsApi->create_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **create_transaction_request** | [**CreateTransactionRequest**](CreateTransactionRequest.md) |  |  |
| **x_idempotency_key** | **String** | Optional unique key for a create request (e.g. a UUID). A retried create with the same key returns the original transaction instead of creating a duplicate — send it on every create so a network retry can&#39;t double-charge the customer.  | [optional] |

### Return type

[**TransactionEnvelope**](TransactionEnvelope.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## get_transaction

> <TransactionEnvelope> get_transaction(transaction_id)

Retrieve a single transaction

### Examples

```ruby
require 'time'
require 'cryptogate'
# setup authorization
CryptoGate.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = CryptoGate::TransactionsApi.new
transaction_id = 'transaction_id_example' # String | 

begin
  # Retrieve a single transaction
  result = api_instance.get_transaction(transaction_id)
  p result
rescue CryptoGate::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction: #{e}"
end
```

#### Using the get_transaction_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<TransactionEnvelope>, Integer, Hash)> get_transaction_with_http_info(transaction_id)

```ruby
begin
  # Retrieve a single transaction
  data, status_code, headers = api_instance.get_transaction_with_http_info(transaction_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <TransactionEnvelope>
rescue CryptoGate::ApiError => e
  puts "Error when calling TransactionsApi->get_transaction_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **transaction_id** | **String** |  |  |

### Return type

[**TransactionEnvelope**](TransactionEnvelope.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_transactions

> <ListTransactions200Response> list_transactions(opts)

List the merchant's transactions (newest first)

### Examples

```ruby
require 'time'
require 'cryptogate'
# setup authorization
CryptoGate.configure do |config|
  # Configure Bearer authorization: SecretKey
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = CryptoGate::TransactionsApi.new
opts = {
  limit: 56, # Integer | 
  offset: 56, # Integer | 
  status: CryptoGate::TransactionStatus::PENDING, # TransactionStatus | 
  crypto: CryptoGate::CryptoSymbol::BTC # CryptoSymbol | 
}

begin
  # List the merchant's transactions (newest first)
  result = api_instance.list_transactions(opts)
  p result
rescue CryptoGate::ApiError => e
  puts "Error when calling TransactionsApi->list_transactions: #{e}"
end
```

#### Using the list_transactions_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ListTransactions200Response>, Integer, Hash)> list_transactions_with_http_info(opts)

```ruby
begin
  # List the merchant's transactions (newest first)
  data, status_code, headers = api_instance.list_transactions_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ListTransactions200Response>
rescue CryptoGate::ApiError => e
  puts "Error when calling TransactionsApi->list_transactions_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **limit** | **Integer** |  | [optional][default to 20] |
| **offset** | **Integer** |  | [optional][default to 0] |
| **status** | [**TransactionStatus**](.md) |  | [optional] |
| **crypto** | [**CryptoSymbol**](.md) |  | [optional] |

### Return type

[**ListTransactions200Response**](ListTransactions200Response.md)

### Authorization

[SecretKey](../README.md#SecretKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

