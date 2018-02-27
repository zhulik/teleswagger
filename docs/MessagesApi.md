# Teleswagger::MessagesApi

All URIs are relative to *https://api.telegram.org/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_message**](MessagesApi.md#delete_message) | **GET** /bot{token}/deleteMessage | 
[**edit_message_caption**](MessagesApi.md#edit_message_caption) | **POST** /bot{token}/editMessageCaption | 
[**edit_message_reply_markup**](MessagesApi.md#edit_message_reply_markup) | **POST** /bot{token}/editMessageReplyMarkup | 
[**edit_message_text**](MessagesApi.md#edit_message_text) | **POST** /bot{token}/editMessageText | 
[**forward_message**](MessagesApi.md#forward_message) | **POST** /bot{token}/forwardMessage | 
[**send_message**](MessagesApi.md#send_message) | **POST** /bot{token}/sendMessage | 
[**send_message_bytes**](MessagesApi.md#send_message_bytes) | **POST** /bot{token}/sendMessage#bytes | 


# **delete_message**
> ResponseBool delete_message(token, chat_id, message_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::MessagesApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

message_id = 56 # Integer | 


begin
  result = api_instance.delete_message(token, chat_id, message_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling MessagesApi->delete_message: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **message_id** | **Integer**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **edit_message_caption**
> InlineResponse200 edit_message_caption(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::MessagesApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::EditMessageCaptionBody.new # EditMessageCaptionBody | 
}

begin
  result = api_instance.edit_message_caption(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling MessagesApi->edit_message_caption: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**EditMessageCaptionBody**](EditMessageCaptionBody.md)|  | [optional] 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **edit_message_reply_markup**
> InlineResponse200 edit_message_reply_markup(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::MessagesApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::EditMessageReplyMarkupBody.new # EditMessageReplyMarkupBody | 
}

begin
  result = api_instance.edit_message_reply_markup(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling MessagesApi->edit_message_reply_markup: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**EditMessageReplyMarkupBody**](EditMessageReplyMarkupBody.md)|  | [optional] 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **edit_message_text**
> InlineResponse200 edit_message_text(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::MessagesApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::EditMessageTextBody.new # EditMessageTextBody | 
}

begin
  result = api_instance.edit_message_text(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling MessagesApi->edit_message_text: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**EditMessageTextBody**](EditMessageTextBody.md)|  | [optional] 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **forward_message**
> ResponseMessage forward_message(token, chat_id, from_chat_id, message_id, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::MessagesApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

from_chat_id = "from_chat_id_example" # String | 

message_id = 56 # Integer | 

opts = { 
  disable_notification: true # BOOLEAN | 
}

begin
  result = api_instance.forward_message(token, chat_id, from_chat_id, message_id, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling MessagesApi->forward_message: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **from_chat_id** | **String**|  | 
 **message_id** | **Integer**|  | 
 **disable_notification** | **BOOLEAN**|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json



# **send_message**
> ResponseMessage send_message(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::MessagesApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendMessageBody.new # SendMessageBody | 
}

begin
  result = api_instance.send_message(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling MessagesApi->send_message: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendMessageBody**](SendMessageBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_message_bytes**
> ResponseMessage send_message_bytes(token, body)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::MessagesApi.new

token = "token_example" # String | bot's token to authorize the request

body = "B" # String | 


begin
  result = api_instance.send_message_bytes(token, body)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling MessagesApi->send_message_bytes: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | **String**|  | 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



