# cloudmersive_cdr_api_client.FileSanitizationApi

All URIs are relative to *https://api.cloudmersive.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**file**](FileSanitizationApi.md#file) | **POST** /cdr/sanitization/file | Complete Content Disarm and Reconstruction on an Input File, and output in same file format
[**file_to_pdf**](FileSanitizationApi.md#file_to_pdf) | **POST** /cdr/sanitization/file/to/pdf | Complete Content Disarm and Reconstruction on an Input File with PDF/A Output


# **file**
> file(input_file=input_file)

Complete Content Disarm and Reconstruction on an Input File, and output in same file format

Processes the input file via CDR to produce a secured output file.  Input content is parsed, disarmed, and then reconstructed into a new output file with the same file format as the input.

### Example
```python
from __future__ import print_function
import time
import cloudmersive_cdr_api_client
from cloudmersive_cdr_api_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: Apikey
configuration = cloudmersive_cdr_api_client.Configuration()
configuration.api_key['Apikey'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Apikey'] = 'Bearer'

# create an instance of the API class
api_instance = cloudmersive_cdr_api_client.FileSanitizationApi(cloudmersive_cdr_api_client.ApiClient(configuration))
input_file = '/path/to/file.txt' # file | Input document, or photos of a document, to extract data from (optional)

try:
    # Complete Content Disarm and Reconstruction on an Input File, and output in same file format
    api_instance.file(input_file=input_file)
except ApiException as e:
    print("Exception when calling FileSanitizationApi->file: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input_file** | **file**| Input document, or photos of a document, to extract data from | [optional] 

### Return type

void (empty response body)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **file_to_pdf**
> file_to_pdf(input_file=input_file)

Complete Content Disarm and Reconstruction on an Input File with PDF/A Output

Processes the input file via CDR to produce a secured PDF/A output file.  Input content is parsed, disarmed, and then reconstructed into a new PDF/A output file.

### Example
```python
from __future__ import print_function
import time
import cloudmersive_cdr_api_client
from cloudmersive_cdr_api_client.rest import ApiException
from pprint import pprint

# Configure API key authorization: Apikey
configuration = cloudmersive_cdr_api_client.Configuration()
configuration.api_key['Apikey'] = 'YOUR_API_KEY'
# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['Apikey'] = 'Bearer'

# create an instance of the API class
api_instance = cloudmersive_cdr_api_client.FileSanitizationApi(cloudmersive_cdr_api_client.ApiClient(configuration))
input_file = '/path/to/file.txt' # file | Input document, or photos of a document, to extract data from (optional)

try:
    # Complete Content Disarm and Reconstruction on an Input File with PDF/A Output
    api_instance.file_to_pdf(input_file=input_file)
except ApiException as e:
    print("Exception when calling FileSanitizationApi->file_to_pdf: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **input_file** | **file**| Input document, or photos of a document, to extract data from | [optional] 

### Return type

void (empty response body)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

