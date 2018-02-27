# Teleswagger::AttachmentsApi

All URIs are relative to *https://api.telegram.org/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**edit_message_live_location**](AttachmentsApi.md#edit_message_live_location) | **POST** /bot{token}/editMessageLiveLocation | 
[**get_file**](AttachmentsApi.md#get_file) | **GET** /bot{token}/getFile | 
[**send_audio**](AttachmentsApi.md#send_audio) | **POST** /bot{token}/sendAudio | 
[**send_audio_link**](AttachmentsApi.md#send_audio_link) | **POST** /bot{token}/sendAudio#link | 
[**send_contact**](AttachmentsApi.md#send_contact) | **POST** /bot{token}/sendContact | 
[**send_document**](AttachmentsApi.md#send_document) | **POST** /bot{token}/sendDocument | 
[**send_document_link**](AttachmentsApi.md#send_document_link) | **POST** /bot{token}/sendDocument#link | 
[**send_location**](AttachmentsApi.md#send_location) | **POST** /bot{token}/sendLocation | 
[**send_media_group_link**](AttachmentsApi.md#send_media_group_link) | **POST** /bot{token}/sendMediaGroup#link | 
[**send_photo**](AttachmentsApi.md#send_photo) | **POST** /bot{token}/sendPhoto | 
[**send_photo_link**](AttachmentsApi.md#send_photo_link) | **POST** /bot{token}/sendPhoto#link | 
[**send_sticker**](AttachmentsApi.md#send_sticker) | **POST** /bot{token}/sendSticker | 
[**send_sticker_link**](AttachmentsApi.md#send_sticker_link) | **POST** /bot{token}/sendSticker#link | 
[**send_venue**](AttachmentsApi.md#send_venue) | **POST** /bot{token}/sendVenue | 
[**send_video**](AttachmentsApi.md#send_video) | **POST** /bot{token}/sendVideo | 
[**send_video_link**](AttachmentsApi.md#send_video_link) | **POST** /bot{token}/sendVideo#link | 
[**send_video_note**](AttachmentsApi.md#send_video_note) | **POST** /bot{token}/sendVideoNote | 
[**send_video_note_link**](AttachmentsApi.md#send_video_note_link) | **POST** /bot{token}/sendVideoNote#link | 
[**send_voice**](AttachmentsApi.md#send_voice) | **POST** /bot{token}/sendVoice | 
[**send_voice_link**](AttachmentsApi.md#send_voice_link) | **POST** /bot{token}/sendVoice#link | 
[**stop_message_live_location**](AttachmentsApi.md#stop_message_live_location) | **POST** /bot{token}/stopMessageLiveLocation | 


# **edit_message_live_location**
> ResponseMessage edit_message_live_location(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::EditMessageLiveLocationBody.new # EditMessageLiveLocationBody | 
}

begin
  result = api_instance.edit_message_live_location(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->edit_message_live_location: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**EditMessageLiveLocationBody**](EditMessageLiveLocationBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **get_file**
> InlineResponse2005 get_file(token, file_id)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

file_id = "file_id_example" # String | 


begin
  result = api_instance.get_file(token, file_id)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->get_file: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **file_id** | **String**|  | 

### Return type

[**InlineResponse2005**](InlineResponse2005.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_audio**
> ResponseMessage send_audio(token, chat_id, audio, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

audio = File.new("/path/to/file.txt") # File | 

opts = { 
  caption: "caption_example", # String | 
  parse_mode: "parse_mode_example", # String | 
  duration: 56, # Integer | 
  performer: "performer_example", # String | 
  title: "title_example", # String | 
  disable_notification: true, # BOOLEAN | 
  reply_to_message_id: 56, # Integer | 
  reply_markup: "reply_markup_example" # String | json string of reply_markup object
}

begin
  result = api_instance.send_audio(token, chat_id, audio, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_audio: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **audio** | **File**|  | 
 **caption** | **String**|  | [optional] 
 **parse_mode** | **String**|  | [optional] 
 **duration** | **Integer**|  | [optional] 
 **performer** | **String**|  | [optional] 
 **title** | **String**|  | [optional] 
 **disable_notification** | **BOOLEAN**|  | [optional] 
 **reply_to_message_id** | **Integer**|  | [optional] 
 **reply_markup** | **String**| json string of reply_markup object | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **send_audio_link**
> ResponseMessage send_audio_link(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendAudioLinkBody.new # SendAudioLinkBody | 
}

begin
  result = api_instance.send_audio_link(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_audio_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendAudioLinkBody**](SendAudioLinkBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_contact**
> ResponseMessage send_contact(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendContactBody.new # SendContactBody | 
}

begin
  result = api_instance.send_contact(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_contact: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendContactBody**](SendContactBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_document**
> ResponseMessage send_document(token, chat_id, document, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

document = File.new("/path/to/file.txt") # File | 

opts = { 
  caption: "caption_example", # String | 
  parse_mode: "parse_mode_example", # String | 
  disable_notification: true, # BOOLEAN | 
  reply_to_message_id: 56, # Integer | 
  reply_markup: "reply_markup_example" # String | json string of reply_markup object
}

begin
  result = api_instance.send_document(token, chat_id, document, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_document: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **document** | **File**|  | 
 **caption** | **String**|  | [optional] 
 **parse_mode** | **String**|  | [optional] 
 **disable_notification** | **BOOLEAN**|  | [optional] 
 **reply_to_message_id** | **Integer**|  | [optional] 
 **reply_markup** | **String**| json string of reply_markup object | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **send_document_link**
> ResponseMessage send_document_link(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendDocumentLinkBody.new # SendDocumentLinkBody | 
}

begin
  result = api_instance.send_document_link(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_document_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendDocumentLinkBody**](SendDocumentLinkBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_location**
> ResponseMessage send_location(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendLocationBody.new # SendLocationBody | 
}

begin
  result = api_instance.send_location(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_location: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendLocationBody**](SendLocationBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_media_group_link**
> ResponseMessage send_media_group_link(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendMediaGroupLinkBody.new # SendMediaGroupLinkBody | 
}

begin
  result = api_instance.send_media_group_link(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_media_group_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendMediaGroupLinkBody**](SendMediaGroupLinkBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_photo**
> ResponseMessage send_photo(token, chat_id, photo, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

photo = File.new("/path/to/file.txt") # File | 

opts = { 
  caption: "caption_example", # String | 
  parse_mode: "parse_mode_example", # String | 
  disable_notification: true, # BOOLEAN | 
  reply_to_message_id: 56, # Integer | 
  reply_markup: "reply_markup_example" # String | json string of reply_markup object
}

begin
  result = api_instance.send_photo(token, chat_id, photo, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_photo: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **photo** | **File**|  | 
 **caption** | **String**|  | [optional] 
 **parse_mode** | **String**|  | [optional] 
 **disable_notification** | **BOOLEAN**|  | [optional] 
 **reply_to_message_id** | **Integer**|  | [optional] 
 **reply_markup** | **String**| json string of reply_markup object | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **send_photo_link**
> ResponseMessage send_photo_link(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendPhotoLinkBody.new # SendPhotoLinkBody | 
}

begin
  result = api_instance.send_photo_link(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_photo_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendPhotoLinkBody**](SendPhotoLinkBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_sticker**
> ResponseMessage send_sticker(token, chat_id, sticker, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

sticker = File.new("/path/to/file.txt") # File | 

opts = { 
  disable_notification: true, # BOOLEAN | 
  reply_to_message_id: 56, # Integer | 
  reply_markup: "reply_markup_example" # String | json string of reply_markup object
}

begin
  result = api_instance.send_sticker(token, chat_id, sticker, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_sticker: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **sticker** | **File**|  | 
 **disable_notification** | **BOOLEAN**|  | [optional] 
 **reply_to_message_id** | **Integer**|  | [optional] 
 **reply_markup** | **String**| json string of reply_markup object | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **send_sticker_link**
> ResponseMessage send_sticker_link(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendStickerLinkBody.new # SendStickerLinkBody | 
}

begin
  result = api_instance.send_sticker_link(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_sticker_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendStickerLinkBody**](SendStickerLinkBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_venue**
> ResponseMessage send_venue(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendVenueBody.new # SendVenueBody | 
}

begin
  result = api_instance.send_venue(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_venue: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendVenueBody**](SendVenueBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_video**
> ResponseMessage send_video(token, chat_id, video, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

video = File.new("/path/to/file.txt") # File | 

opts = { 
  duration: 56, # Integer | 
  width: 56, # Integer | 
  height: 56, # Integer | 
  caption: "caption_example", # String | 
  parse_mode: "parse_mode_example", # String | 
  disable_notification: true, # BOOLEAN | 
  reply_to_message_id: 56, # Integer | 
  reply_markup: "reply_markup_example" # String | json string of reply_markup object
}

begin
  result = api_instance.send_video(token, chat_id, video, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_video: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **video** | **File**|  | 
 **duration** | **Integer**|  | [optional] 
 **width** | **Integer**|  | [optional] 
 **height** | **Integer**|  | [optional] 
 **caption** | **String**|  | [optional] 
 **parse_mode** | **String**|  | [optional] 
 **disable_notification** | **BOOLEAN**|  | [optional] 
 **reply_to_message_id** | **Integer**|  | [optional] 
 **reply_markup** | **String**| json string of reply_markup object | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **send_video_link**
> ResponseMessage send_video_link(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendVideoLinkBody.new # SendVideoLinkBody | 
}

begin
  result = api_instance.send_video_link(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_video_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendVideoLinkBody**](SendVideoLinkBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_video_note**
> ResponseMessage send_video_note(token, chat_id, video_note, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

video_note = File.new("/path/to/file.txt") # File | 

opts = { 
  duration: 56, # Integer | 
  length: 56, # Integer | 
  disable_notification: true, # BOOLEAN | 
  reply_to_message_id: 56, # Integer | 
  reply_markup: "reply_markup_example" # String | json string of reply_markup object
}

begin
  result = api_instance.send_video_note(token, chat_id, video_note, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_video_note: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **video_note** | **File**|  | 
 **duration** | **Integer**|  | [optional] 
 **length** | **Integer**|  | [optional] 
 **disable_notification** | **BOOLEAN**|  | [optional] 
 **reply_to_message_id** | **Integer**|  | [optional] 
 **reply_markup** | **String**| json string of reply_markup object | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **send_video_note_link**
> ResponseMessage send_video_note_link(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendVideoNoteLinkBody.new # SendVideoNoteLinkBody | 
}

begin
  result = api_instance.send_video_note_link(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_video_note_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendVideoNoteLinkBody**](SendVideoNoteLinkBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **send_voice**
> ResponseMessage send_voice(token, chat_id, voice, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

chat_id = "chat_id_example" # String | 

voice = File.new("/path/to/file.txt") # File | 

opts = { 
  caption: "caption_example", # String | 
  parse_mode: "parse_mode_example", # String | 
  duration: 56, # Integer | 
  disable_notification: true, # BOOLEAN | 
  reply_to_message_id: 56, # Integer | 
  reply_markup: "reply_markup_example" # String | json string of reply_markup object
}

begin
  result = api_instance.send_voice(token, chat_id, voice, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_voice: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **chat_id** | **String**|  | 
 **voice** | **File**|  | 
 **caption** | **String**|  | [optional] 
 **parse_mode** | **String**|  | [optional] 
 **duration** | **Integer**|  | [optional] 
 **disable_notification** | **BOOLEAN**|  | [optional] 
 **reply_to_message_id** | **Integer**|  | [optional] 
 **reply_markup** | **String**| json string of reply_markup object | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **send_voice_link**
> ResponseMessage send_voice_link(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::SendVoiceLinkBody.new # SendVoiceLinkBody | 
}

begin
  result = api_instance.send_voice_link(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->send_voice_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**SendVoiceLinkBody**](SendVoiceLinkBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **stop_message_live_location**
> ResponseMessage stop_message_live_location(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::AttachmentsApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  body: Teleswagger::StopMessageLiveLocationBody.new # StopMessageLiveLocationBody | 
}

begin
  result = api_instance.stop_message_live_location(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling AttachmentsApi->stop_message_live_location: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**StopMessageLiveLocationBody**](StopMessageLiveLocationBody.md)|  | [optional] 

### Return type

[**ResponseMessage**](ResponseMessage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



