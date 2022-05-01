# DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**isPhoneRegPost**](DefaultApi.md#isPhoneRegPost) | **POST** /IsPhoneReg | 检查手机号是否注册
[**juguguLoginCodeandReturnInfoPost**](DefaultApi.md#juguguLoginCodeandReturnInfoPost) | **POST** /Jugugu_LoginCodeandReturnInfo | ①获取验证码图片
[**jugugugRegAndVerifyandReturnInfoPost**](DefaultApi.md#jugugugRegAndVerifyandReturnInfoPost) | **POST** /Jugugug_RegAndVerifyandReturnInfo | ③注册Jugugu


<a name="isPhoneRegPost"></a>
# **isPhoneRegPost**
> InlineResponse200 isPhoneRegPost(inlineObject)

检查手机号是否注册

检查手机号是否注册，返回“true”和“false”字符串

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    InlineObject inlineObject = new InlineObject(); // InlineObject | 
    try {
      InlineResponse200 result = apiInstance.isPhoneRegPost(inlineObject);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#isPhoneRegPost");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject** | [**InlineObject**](InlineObject.md)|  | [optional]

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

<a name="juguguLoginCodeandReturnInfoPost"></a>
# **juguguLoginCodeandReturnInfoPost**
> InlineResponse2001 juguguLoginCodeandReturnInfoPost(inlineObject2)

①获取验证码图片

获取用于防御机器人的验证码图片，phone的传参必须为空字符串

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    InlineObject2 inlineObject2 = new InlineObject2(); // InlineObject2 | 
    try {
      InlineResponse2001 result = apiInstance.juguguLoginCodeandReturnInfoPost(inlineObject2);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#juguguLoginCodeandReturnInfoPost");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject2** | [**InlineObject2**](InlineObject2.md)|  | [optional]

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

<a name="jugugugRegAndVerifyandReturnInfoPost"></a>
# **jugugugRegAndVerifyandReturnInfoPost**
> InlineResponse2001 jugugugRegAndVerifyandReturnInfoPost(inlineObject1)

③注册Jugugu

注册jugugu，注意三点 1.phone的传参必须为11位的国内手机号。 2.robotcodeid和robotcode是通过【①】获得 3.code短信验证码通过【②】 4.paymentpassword区块链短密钥，该密钥为用户进行链上交互使用，密钥设置长度&gt;9位，且包含0-1 A-B a-b 已经特殊字符[~!@#$%^&amp;*?_+;&#39;,./\\|·！￥（）{}：“《》？、，。；’”\&quot;《》…-]+

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.DefaultApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("http://localhost");

    DefaultApi apiInstance = new DefaultApi(defaultClient);
    InlineObject1 inlineObject1 = new InlineObject1(); // InlineObject1 | 
    try {
      InlineResponse2001 result = apiInstance.jugugugRegAndVerifyandReturnInfoPost(inlineObject1);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling DefaultApi#jugugugRegAndVerifyandReturnInfoPost");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject1** | [**InlineObject1**](InlineObject1.md)|  | [optional]

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | 成功 |  -  |

