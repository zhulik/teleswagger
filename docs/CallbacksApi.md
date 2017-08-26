# Teleswagger::CallbacksApi

All URIs are relative to *https://api.telegram.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**answer_callback_query**](CallbacksApi.md#answer_callback_query) | **POST** /bot{token}/answerCallbackQuery | 


# **answer_callback_query**
> ResponseBool answer_callback_query(token, callback_query_id, text, show_alert, url, cache_time)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::CallbacksApi.new

token = "token_example" # String | bot's token to authorize the request

callback_query_id = "callback_query_id_example" # String | 

text = "text_example" # String | 

show_alert = true # BOOLEAN | 

url = "url_example" # String | 

cache_time = 56 # Integer | 


begin
  result = api_instance.answer_callback_query(token, callback_query_id, text, show_alert, url, cache_time)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling CallbacksApi->answer_callback_query: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **callback_query_id** | **String**|  | 
 **text** | **String**|  | 
 **show_alert** | **BOOLEAN**|  | 
 **url** | **String**|  | 
 **cache_time** | **Integer**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json



