# Teleswagger::InlineApi

All URIs are relative to *https://api.telegram.org/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**answer_inline_query**](InlineApi.md#answer_inline_query) | **POST** /bot{token}/answerInlineQuery | 


# **answer_inline_query**
> ResponseBool answer_inline_query(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::InlineApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::AnswerInlineQueryBody.new # AnswerInlineQueryBody | 
}

begin
  result = api_instance.answer_inline_query(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling InlineApi->answer_inline_query: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**AnswerInlineQueryBody**](AnswerInlineQueryBody.md)|  | [optional] 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



