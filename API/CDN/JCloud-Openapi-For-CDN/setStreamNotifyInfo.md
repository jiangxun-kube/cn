# setStreamNotifyInfo


## 描述
设置推流中断通知方式

## 请求方式
POST

## 请求地址
https://cdn.jdcloud-api.com/v1/liveDomain/{domain}/streamNotifyInfo

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**domain**|String|True| |用户域名|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**notifyUrl**|String|True| |通知的目标URL|
|**notifyAuthKey**|String|True| |通知时需携带的鉴权key|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**result**|[Result](#result)| |
|**requestId**|String| |

### <div id="Result">Result</div>
|名称|类型|描述|
|---|---|---|
|**ignoreQueryString**|String|是否忽略参数|
|**pushIpWhiteList**|String|推流IP白名单（用逗号分隔）|
|**publishNormalTimeout**|Integer|推流超时时间|
|**notifyCustomUrl**|String|推断流时，通知客户系统的URL|
|**notifyCustomAuthKey**|String|通知客户系统的鉴权key|
|**forwardAccessKeyType**|Integer|转推鉴权类型（0：不鉴权，1：参数鉴权，2：URL鉴权）|
|**forwardPrivateKey**|String|转推的鉴权key|
|**originAccessKeyType**|Integer|回源鉴权类型（0：不鉴权，1：参数鉴权，2：URL鉴权）|
|**originPrivateKey**|String|回源的鉴权key|

## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
|**404**|NOT_FOUND|
