# Teleswagger::PaymentsApi

All URIs are relative to *https://api.telegram.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**answer_pre_checkout_query**](PaymentsApi.md#answer_pre_checkout_query) | **GET** /bot{token}/answerPreCheckoutQuery | 
[**answer_shipping_query**](PaymentsApi.md#answer_shipping_query) | **POST** /bot{token}/answerShippingQuery | 
[**send_invoice**](PaymentsApi.md#send_invoice) | **POST** /bot{token}/sendInvoice | 


# **answer_pre_checkout_query**
> ResponseBool answer_pre_checkout_query(token, pre_checkout_query_id, ok, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::PaymentsApi.new

token = "token_example" # String | bot's token to authorize the request

pre_checkout_query_id = "pre_checkout_query_id_example" # String | 

ok = true # BOOLEAN | 

opts = { 
  error_message: "error_message_example" # String | 
}

begin
  result = api_instance.answer_pre_checkout_query(token, pre_checkout_query_id, ok, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling PaymentsApi->answer_pre_checkout_query: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **pre_checkout_query_id** | **String**|  | 
 **ok** | **BOOLEAN**|  | 
 **error_message** | **String**|  | [optional] 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **answer_shipping_query**
> ResponseMessage answer_shipping_query(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::PaymentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::AnswerShippingQueryBody.new # AnswerShippingQueryBody | 
}

begin
  result = api_instance.answer_shipping_query(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling PaymentsApi->answer_shipping_query: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**AnswerShippingQueryBody**](AnswerShippingQueryBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_invoice**
> ResponseMessage send_invoice(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::PaymentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendInvoiceBody.new # SendInvoiceBody | 
}

begin
  result = api_instance.send_invoice(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling PaymentsApi->send_invoice: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendInvoiceBody**](SendInvoiceBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



