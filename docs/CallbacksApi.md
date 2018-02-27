# Teleswagger::CallbacksApi

All URIs are relative to *https://api.telegram.org/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**answer_callback_query**](CallbacksApi.md#answer_callback_query) | **POST** /bot{token}/answerCallbackQuery | 


# **answer_callback_query**
> ResponseBool answer_callback_query(token, body)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::CallbacksApi.new

token = "token_example" # String | bot's token to authorize the request

body = Teleswagger::AnswerCallbackQueryBody.new # AnswerCallbackQueryBody | 


begin
  result = api_instance.answer_callback_query(token, body)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling CallbacksApi->answer_callback_query: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**AnswerCallbackQueryBody**](AnswerCallbackQueryBody.md)|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



