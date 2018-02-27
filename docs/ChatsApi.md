# Teleswagger::ChatsApi

All URIs are relative to *https://api.telegram.org/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_chat_photo**](ChatsApi.md#delete_chat_photo) | **POST** /bot{token}/deleteChatPhoto | 
[**delete_chat_sticker_set**](ChatsApi.md#delete_chat_sticker_set) | **GET** /bot{token}/deleteChatStickerSet | 
[**export_chat_invite_link**](ChatsApi.md#export_chat_invite_link) | **GET** /bot{token}/exportChatInviteLink | 
[**get_chat**](ChatsApi.md#get_chat) | **GET** /bot{token}/getChat | 
[**get_chat_administrators**](ChatsApi.md#get_chat_administrators) | **GET** /bot{token}/getChatAdministrators | 
[**get_chat_member**](ChatsApi.md#get_chat_member) | **GET** /bot{token}/getChatMember | 
[**get_chat_members_count**](ChatsApi.md#get_chat_members_count) | **GET** /bot{token}/getChatMembersCount | 
[**kick_chat_member**](ChatsApi.md#kick_chat_member) | **GET** /bot{token}/kickChatMember | 
[**leave_chat**](ChatsApi.md#leave_chat) | **GET** /bot{token}/leaveChat | 
[**pin_chat_message**](ChatsApi.md#pin_chat_message) | **POST** /bot{token}/pinChatMessage | 
[**promote_chat_member**](ChatsApi.md#promote_chat_member) | **POST** /bot{token}/promoteChatMember | 
[**restrict_chat_member**](ChatsApi.md#restrict_chat_member) | **POST** /bot{token}/restrictChatMember | 
[**send_chat_action**](ChatsApi.md#send_chat_action) | **GET** /bot{token}/sendChatAction | 
[**set_chat_description**](ChatsApi.md#set_chat_description) | **POST** /bot{token}/setChatDescription | 
[**set_chat_photo**](ChatsApi.md#set_chat_photo) | **GET** /bot{token}/setChatPhoto | 
[**set_chat_sticker_set**](ChatsApi.md#set_chat_sticker_set) | **GET** /bot{token}/setChatStickerSet | 
[**set_chat_title**](ChatsApi.md#set_chat_title) | **POST** /bot{token}/setChatTitle | 
[**unban_chat_member**](ChatsApi.md#unban_chat_member) | **GET** /bot{token}/unbanChatMember | 
[**unpin_chat_message**](ChatsApi.md#unpin_chat_message) | **POST** /bot{token}/unpinChatMessage | 


# **delete_chat_photo**
> ResponseBool delete_chat_photo(token, chat_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 


begin
  result = api_instance.delete_chat_photo(token, chat_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->delete_chat_photo: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **delete_chat_sticker_set**
> ResponseBool delete_chat_sticker_set(token, chat_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 


begin
  result = api_instance.delete_chat_sticker_set(token, chat_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->delete_chat_sticker_set: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **export_chat_invite_link**
> String export_chat_invite_link(token, chat_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 


begin
  result = api_instance.export_chat_invite_link(token, chat_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->export_chat_invite_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **get_chat**
> InlineResponse2001 get_chat(token, chat_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 


begin
  result = api_instance.get_chat(token, chat_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->get_chat: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **get_chat_administrators**
> InlineResponse2002 get_chat_administrators(token, chat_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 


begin
  result = api_instance.get_chat_administrators(token, chat_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->get_chat_administrators: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 

### Return type

[**InlineResponse2002**](InlineResponse2002.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **get_chat_member**
> InlineResponse2003 get_chat_member(token, chat_id, user_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

user_id = "user_id_example" # String | 


begin
  result = api_instance.get_chat_member(token, chat_id, user_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->get_chat_member: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **user_id** | **String**|  | 

### Return type

[**InlineResponse2003**](InlineResponse2003.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **get_chat_members_count**
> InlineResponse2004 get_chat_members_count(token, chat_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 


begin
  result = api_instance.get_chat_members_count(token, chat_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->get_chat_members_count: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 

### Return type

[**InlineResponse2004**](InlineResponse2004.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **kick_chat_member**
> ResponseBool kick_chat_member(token, chat_id, user_id, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

user_id = 56 # Integer | 

opts = { 
  until_date: 56 # Integer | 
}

begin
  result = api_instance.kick_chat_member(token, chat_id, user_id, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->kick_chat_member: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **user_id** | **Integer**|  | 
 **until_date** | **Integer**|  | [optional] 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **leave_chat**
> ResponseBool leave_chat(token, chat_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 


begin
  result = api_instance.leave_chat(token, chat_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->leave_chat: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **pin_chat_message**
> ResponseBool pin_chat_message(token, chat_id, message_id, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

message_id = 56 # Integer | 

opts = { 
  disable_notification: true # BOOLEAN | 
}

begin
  result = api_instance.pin_chat_message(token, chat_id, message_id, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->pin_chat_message: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **message_id** | **Integer**|  | 
 **disable_notification** | **BOOLEAN**|  | [optional] 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **promote_chat_member**
> ResponseBool promote_chat_member(token, body)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

body = Teleswagger::PromoteChatMemberBody.new # PromoteChatMemberBody | 


begin
  result = api_instance.promote_chat_member(token, body)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->promote_chat_member: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**PromoteChatMemberBody**](PromoteChatMemberBody.md)|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **restrict_chat_member**
> ResponseBool restrict_chat_member(token, body)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

body = Teleswagger::RestrictChatMemberBody.new # RestrictChatMemberBody | 


begin
  result = api_instance.restrict_chat_member(token, body)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->restrict_chat_member: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**RestrictChatMemberBody**](RestrictChatMemberBody.md)|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_chat_action**
> ResponseBool send_chat_action(token, chat_id, action)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

action = "action_example" # String | 


begin
  result = api_instance.send_chat_action(token, chat_id, action)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->send_chat_action: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **action** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **set_chat_description**
> ResponseBool set_chat_description(token, chat_id, description)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

description = "description_example" # String | 


begin
  result = api_instance.set_chat_description(token, chat_id, description)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->set_chat_description: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **description** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **set_chat_photo**
> ResponseBool set_chat_photo(token, chat_id, photo)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

photo = File.new("/path/to/file.txt") # File | 


begin
  result = api_instance.set_chat_photo(token, chat_id, photo)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->set_chat_photo: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **photo** | **File**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **set_chat_sticker_set**
> ResponseBool set_chat_sticker_set(token, chat_id, sticker_set_name)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

sticker_set_name = "sticker_set_name_example" # String | 


begin
  result = api_instance.set_chat_sticker_set(token, chat_id, sticker_set_name)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->set_chat_sticker_set: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **sticker_set_name** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **set_chat_title**
> ResponseBool set_chat_title(token, chat_id, title)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

title = "title_example" # String | 


begin
  result = api_instance.set_chat_title(token, chat_id, title)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->set_chat_title: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **title** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **unban_chat_member**
> ResponseBool unban_chat_member(token, chat_id, user_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

user_id = "user_id_example" # String | 


begin
  result = api_instance.unban_chat_member(token, chat_id, user_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->unban_chat_member: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **user_id** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **unpin_chat_message**
> ResponseBool unpin_chat_message(token, chat_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::ChatsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 


begin
  result = api_instance.unpin_chat_message(token, chat_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling ChatsApi->unpin_chat_message: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



