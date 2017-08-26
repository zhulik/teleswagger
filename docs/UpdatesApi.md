# Teleswagger::UpdatesApi

All URIs are relative to *https://api.telegram.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_webhook**](UpdatesApi.md#delete_webhook) | **GET** /bot{token}/deleteWebhook | 
[**get_updates**](UpdatesApi.md#get_updates) | **GET** /bot{token}/getUpdates | 
[**get_webhook_info**](UpdatesApi.md#get_webhook_info) | **GET** /bot{token}/getWebhookInfo | 
[**set_webhook**](UpdatesApi.md#set_webhook) | **POST** /bot{token}/setWebhook | 


# **delete_webhook**
> ResponseBool delete_webhook





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::UpdatesApi.new

begin
  result = api_instance.delete_webhook
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling UpdatesApi->delete_webhook: #{e}"
end
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **get_updates**
> ResponseUpdate get_updates(token, , opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::UpdatesApi.new

token = "token_example" # String | bot's token to authorize the request

opts = { 
  offset: 56, # Integer | 
  limit: 56, # Integer | 
  timeout: 56, # Integer | 
  allowed_updates: ["allowed_updates_example"] # Array<String> | 
}

begin
  result = api_instance.get_updates(token, , opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling UpdatesApi->get_updates: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **offset** | **Integer**|  | [optional] 
 **limit** | **Integer**|  | [optional] 
 **timeout** | **Integer**|  | [optional] 
 **allowed_updates** | [**Array&lt;String&gt;**](String.md)|  | [optional] 

### Return type

[**ResponseUpdate**](ResponseUpdate.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **get_webhook_info**
> WebhookInfo get_webhook_info





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::UpdatesApi.new

begin
  result = api_instance.get_webhook_info
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling UpdatesApi->get_webhook_info: #{e}"
end
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**WebhookInfo**](WebhookInfo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json



# **set_webhook**
> ResponseBool set_webhook(token, url, opts)





### Example
```ruby
# load the gem
require 'teleswagger'

api_instance = Teleswagger::UpdatesApi.new

token = "token_example" # String | bot's token to authorize the request

url = "url_example" # String | 

opts = { 
  certificate: File.new("/path/to/file.txt"), # File | 
  max_connections: 56, # Integer | 
  allowed_updates: ["allowed_updates_example"] # Array<String> | 
}

begin
  result = api_instance.set_webhook(token, url, opts)
  p result
rescue Teleswagger::ApiError => e
  puts "Exception when calling UpdatesApi->set_webhook: #{e}"
end
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **String**| bot&#39;s token to authorize the request | 
 **url** | **String**|  | 
 **certificate** | **File**|  | [optional] 
 **max_connections** | **Integer**|  | [optional] 
 **allowed_updates** | [**Array&lt;String&gt;**](String.md)|  | [optional] 

### Return type

[**ResponseBool**](ResponseBool.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json



