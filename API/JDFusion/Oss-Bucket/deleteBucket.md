# deleteBucket


## 描述
删除指定ID的OSS存储桶信息

## 请求方式
DELETE

## 请求地址
https://jdfusion.jdcloud-api.com/v1/regions/{regionId}/oss_buckets/{name}

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**name**|String|True| |OSS存储桶名称|
|**regionId**|String|True| |地域ID|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**x-jdcloud-fusion-cloudid**|String|False| |云注册信息ID|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**requestId**|String|请求ID|


## 返回码
|返回码|描述|
|---|---|
|**204**|OK|
|**404**|OSS bucket not found|
