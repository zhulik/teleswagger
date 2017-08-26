# Teleswagger::UsersApi

All URIs are relative to *https://api.telegram.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_me**](UsersApi.md#get_me) | **GET** /bot{token}/getMe | 
[**get_user_profile_photos**](UsersApi.md#get_user_profile_photos) | **GET** /bot{token}/getUserProfilePhotos | 


# **get_me**
> InlineResponse200 get_me(token, )





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::UsersApi.new

token = "token_example" # String | bot's token to authorize the request


begin
  result = api_instance.get_me(token, )
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling UsersApi->get_me: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **get_user_profile_photos**
> InlineResponse2001 get_user_profile_photos(token, user_id, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::UsersApi.new

token = "token_example" # String | bot's token to authorize the request

user_id = 56 # Integer | 

opts = { 
  offset: 56, # Integer | 
  limit: 56 # Integer | 
}

begin
  result = api_instance.get_user_profile_photos(token, user_id, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling UsersApi->get_user_profile_photos: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **user_id** | **Integer**|  | 
 **offset** | **Integer**|  | [optional] 
 **limit** | **Integer**|  | [optional] 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



