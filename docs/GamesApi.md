# Teleswagger::GamesApi

All URIs are relative to *https://api.telegram.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_game_high_scores**](GamesApi.md#get_game_high_scores) | **GET** /bot{token}/getGameHighScores | 
[**send_game**](GamesApi.md#send_game) | **POST** /bot{token}/sendGame | 
[**set_game_score**](GamesApi.md#set_game_score) | **GET** /bot{token}/setGameScore | 


# **get_game_high_scores**
> InlineResponse2008 get_game_high_scores(token, user_id, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::GamesApi.new

token = "token_example" # String | bot's token to authorize the request

user_id = 56 # Integer | 

opts = { 
  chat_id: 56, # Integer | 
  message_id: 56, # Integer | 
  inline_message_id: "inline_message_id_example" # String | 
}

begin
  result = api_instance.get_game_high_scores(token, user_id, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling GamesApi->get_game_high_scores: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **user_id** | **Integer**|  | 
 **chat_id** | **Integer**|  | [optional] 
 **message_id** | **Integer**|  | [optional] 
 **inline_message_id** | **String**|  | [optional] 

### Return type

[**InlineResponse2008**](InlineResponse2008.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_game**
> ResponseMessage send_game(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::GamesApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendGameBody.new # SendGameBody | 
}

begin
  result = api_instance.send_game(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling GamesApi->send_game: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendGameBody**](SendGameBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **set_game_score**
> InlineResponse2007 set_game_score(token, user_id, score, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::GamesApi.new

token = "token_example" # String | bot's token to authorize the request

user_id = 56 # Integer | 

score = 56 # Integer | 

opts = { 
  force: true, # BOOLEAN | 
  disable_edit_message: true, # BOOLEAN | 
  chat_id: 56, # Integer | 
  message_id: 56, # Integer | 
  inline_message_id: "inline_message_id_example" # String | 
}

begin
  result = api_instance.set_game_score(token, user_id, score, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling GamesApi->set_game_score: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **user_id** | **Integer**|  | 
 **score** | **Integer**|  | 
 **force** | **BOOLEAN**|  | [optional] 
 **disable_edit_message** | **BOOLEAN**|  | [optional] 
 **chat_id** | **Integer**|  | [optional] 
 **message_id** | **Integer**|  | [optional] 
 **inline_message_id** | **String**|  | [optional] 

### Return type

[**InlineResponse2007**](InlineResponse2007.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



