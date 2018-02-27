# Teleswagger::StickersApi

All URIs are relative to *https://api.telegram.org/*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_sticker_to_set**](StickersApi.md#add_sticker_to_set) | **POST** /bot{token}/addStickerToSet | 
[**add_sticker_to_set_link**](StickersApi.md#add_sticker_to_set_link) | **POST** /bot{token}/addStickerToSet#link | 
[**create_new_sticker_set**](StickersApi.md#create_new_sticker_set) | **POST** /bot{token}/createNewStickerSet | 
[**create_new_sticker_set_link**](StickersApi.md#create_new_sticker_set_link) | **POST** /bot{token}/createNewStickerSet#link | 
[**delete_sticker_from_set**](StickersApi.md#delete_sticker_from_set) | **POST** /bot{token}/deleteStickerFromSet | 
[**get_sticker_set**](StickersApi.md#get_sticker_set) | **GET** /bot{token}/getStickerSet | 
[**set_sticker_position_in_set**](StickersApi.md#set_sticker_position_in_set) | **POST** /bot{token}/setStickerPositionInSet | 
[**upload_sticker_file**](StickersApi.md#upload_sticker_file) | **POST** /bot{token}/uploadStickerFile | 
[**upload_sticker_file_link**](StickersApi.md#upload_sticker_file_link) | **POST** /bot{token}/uploadStickerFile#link | 


# **add_sticker_to_set**
> ResponseBool add_sticker_to_set(token, user_id, name, png_sticker, emojis, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::StickersApi.new

token = "token_example" # String | bot's token to authorize the request

user_id = 56 # Integer | 

name = "name_example" # String | 

png_sticker = File.new("/path/to/file.txt") # File | 

emojis = "emojis_example" # String | 

opts = { 
  mask_position: "mask_position_example" # String | Serialized to JSON MaskPosition
}

begin
  result = api_instance.add_sticker_to_set(token, user_id, name, png_sticker, emojis, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling StickersApi->add_sticker_to_set: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **user_id** | **Integer**|  | 
 **name** | **String**|  | 
 **png_sticker** | **File**|  | 
 **emojis** | **String**|  | 
 **mask_position** | **String**| Serialized to JSON MaskPosition | [optional] 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **add_sticker_to_set_link**
> ResponseBool add_sticker_to_set_link(token, body)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::StickersApi.new

token = "token_example" # String | bot's token to authorize the request

body = Teleswagger::AddStickerToSetLinkBody.new # AddStickerToSetLinkBody | 


begin
  result = api_instance.add_sticker_to_set_link(token, body)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling StickersApi->add_sticker_to_set_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**AddStickerToSetLinkBody**](AddStickerToSetLinkBody.md)|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **create_new_sticker_set**
> File create_new_sticker_set(token, user_id, name, title, png_sticker, emojis, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::StickersApi.new

token = "token_example" # String | bot's token to authorize the request

user_id = 56 # Integer | 

name = "name_example" # String | 

title = "title_example" # String | 

png_sticker = File.new("/path/to/file.txt") # File | 

emojis = "emojis_example" # String | 

opts = { 
  is_masks: true, # BOOLEAN | 
  mask_position: "mask_position_example" # String | Serialized to JSON MaskPosition
}

begin
  result = api_instance.create_new_sticker_set(token, user_id, name, title, png_sticker, emojis, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling StickersApi->create_new_sticker_set: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **user_id** | **Integer**|  | 
 **name** | **String**|  | 
 **title** | **String**|  | 
 **png_sticker** | **File**|  | 
 **emojis** | **String**|  | 
 **is_masks** | **BOOLEAN**|  | [optional] 
 **mask_position** | **String**| Serialized to JSON MaskPosition | [optional] 

### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **create_new_sticker_set_link**
> File create_new_sticker_set_link(token, body)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::StickersApi.new

token = "token_example" # String | bot's token to authorize the request

body = Teleswagger::CreateNewStickerSetLinkBody.new # CreateNewStickerSetLinkBody | 


begin
  result = api_instance.create_new_sticker_set_link(token, body)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling StickersApi->create_new_sticker_set_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **body** | [**CreateNewStickerSetLinkBody**](CreateNewStickerSetLinkBody.md)|  | 

### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **delete_sticker_from_set**
> ResponseBool delete_sticker_from_set(token, sticker)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::StickersApi.new

token = "token_example" # String | bot's token to authorize the request

sticker = "sticker_example" # String | 


begin
  result = api_instance.delete_sticker_from_set(token, sticker)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling StickersApi->delete_sticker_from_set: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **sticker** | **String**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **get_sticker_set**
> InlineResponse2008 get_sticker_set(token, name)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::StickersApi.new

token = "token_example" # String | bot's token to authorize the request

name = "name_example" # String | 


begin
  result = api_instance.get_sticker_set(token, name)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling StickersApi->get_sticker_set: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **name** | **String**|  | 

### Return type

[**InlineResponse2008**](InlineResponse2008.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **set_sticker_position_in_set**
> ResponseBool set_sticker_position_in_set(token, sticker, position)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::StickersApi.new

token = "token_example" # String | bot's token to authorize the request

sticker = "sticker_example" # String | 

position = 56 # Integer | 


begin
  result = api_instance.set_sticker_position_in_set(token, sticker, position)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling StickersApi->set_sticker_position_in_set: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **sticker** | **String**|  | 
 **position** | **Integer**|  | 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **upload_sticker_file**
> File upload_sticker_file(token, user_id, png_sticker)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::StickersApi.new

token = "token_example" # String | bot's token to authorize the request

user_id = 56 # Integer | 

png_sticker = File.new("/path/to/file.txt") # File | 


begin
  result = api_instance.upload_sticker_file(token, user_id, png_sticker)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling StickersApi->upload_sticker_file: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **user_id** | **Integer**|  | 
 **png_sticker** | **File**|  | 

### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



# **upload_sticker_file_link**
> File upload_sticker_file_link(token, user_id, png_sticker)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::StickersApi.new

token = "token_example" # String | bot's token to authorize the request

user_id = 56 # Integer | 

png_sticker = "png_sticker_example" # String | 


begin
  result = api_instance.upload_sticker_file_link(token, user_id, png_sticker)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling StickersApi->upload_sticker_file_link: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **user_id** | **Integer**|  | 
 **png_sticker** | **String**|  | 

### Return type

**File**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



