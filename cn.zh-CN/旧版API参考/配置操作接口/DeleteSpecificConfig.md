# DeleteSpecificConfig {#doc_api_Cdn_DeleteSpecificConfig .reference}

调用DeleteSpecificConfig接口删除加速域名的配置。

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=Cdn&api=DeleteSpecificConfig&type=RPC&version=2014-11-11)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|是|DeleteSpecificConfig|操作接口名，系统规定参数。取值：**DeleteSpecificConfig**。

 |
|DomainName|String|是|www.macaron.org.cn|您的加速域名。

 |
|ConfigId|String|是|2317|配置ID，多个用逗号（,）隔开。

 |
|FunctionName|String|是|error\_page|功能名称。

 |

功能说明。

|名称

|描述

|
|----|----|
|referer\_white\_list\_set

|refer白名单

|
|referer\_black\_list\_set

|refer黑名单

|
|filetype\_based\_ttl\_set

|文件过期时间设置

|
|path\_based\_ttl\_set

|目录过期时间设置

|
|cc\_defense

|防CC攻击

|
|oss\_auth

|OSS鉴权Bucket

|
|ip\_black\_list\_set

|IP黑名单

|
|ip\_white\_list\_set

|IP白名单

|
|error\_page

|错误页面重定向

|
|tesla

|页面优化加速

|
|set\_req\_host\_header

|修改回源自定义头

|
|set\_hashkey\_args

|忽略url参数

|
|aliauth

|阿里鉴权

|
|set\_resp\_header

|设置响应头（浏览器端可见）

|
|video\_seek

|视频切片拖拽开关

|
|range

|Range请求功能

|
|gzip

|页面Gzip优化

|
|https\_force

|强制HTTPS跳转

|
|http\_force

|强制HTTP跳转

|
|alilive

|视频直播配置

|
|forward\_scheme

|静态协议跟随回源

|
|set\_req\_header

|修改回源自定义头

|

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|04F0F334-1335-436C-A1D7-6C044FE73368|请求ID。

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}
http(s)://cdn.aliyuncs.com?Action=DeleteSpecificConfig
&DomainName=www.macaron.org.cn
&ConfigId=2317
&FunctionName=error_page
&<公共请求参数>
```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<DeleteSpecificConfigResponse>
	  <RequestId>04F0F334-1335-436C-A1D7-6C044FE73368</RequestId>
</DeleteSpecificConfigResponse>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"RequestId":"04F0F334-1335-436C-A1D7-6C044FE73368"
}
```

## 错误码 { .section}

|HttpCode|错误码|错误信息|描述|
|--------|---|----|--|
|400|Invalid%s.ValueNotSupported|FunctionName \[%s\] is not supported.|此方法不支持。|
|400|MissingParameter|The specified value of parameter DomainName can not be empty.|参数DomainName不能为空。|
|400|MissingParameter|The specified value of parameter FunctionName can not be empty.|参数FunctionName不能为空。|
|400|MissingParameter|The specified value of parameter ConfigId can not be empty.|参数ConfigId不能为空。|

访问[错误中心](https://error-center.aliyun.com/status/product/Cdn)查看更多错误码。

