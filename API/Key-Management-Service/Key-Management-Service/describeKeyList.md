# describeKeyList


## 描述
获取密钥列表

## 请求方式
GET

## 请求地址
https://kms.jdcloud-api.com/v1/key


## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**pageNumber**|Integer|False|1|页码；默认为1|
|**pageSize**|Integer|False|10|分页大小；默认为10；取值范围[10, 100]|


## 返回参数
|名称|类型|描述|
|---|---|---|
|**result**|[Result](#result)| |
|**requestId**|String|请求ID|

### <div id="Result">Result</div>
|名称|类型|描述|
|---|---|---|
|**keyList**|[KeyInfo[]](#keyinfo)|Key列表|
|**totalCount**|Integer|Key的数量|
### <div id="KeyInfo">KeyInfo</div>
|名称|类型|描述|
|---|---|---|
|**keyId**|String|KeyID|
|**keyName**|String|Key名称|
|**keyStatus**|Integer|Key当前状态: 0:已启用、1:已禁用、2:计划删除|
|**createTime**|String|Key创建时间，采用ISO8601标准，格式为: YYYY-MM-DDTHH:mm:ssZ|
|**keyDesc**|String|Key的用途|
|**rotationCycle**|Integer|Key的轮换周期，为0则永久不轮换|
|**deleteTime**|String|计划删除的时间，采用ISO8601标准，格式为: YYYY-MM-DDTHH:mm:ssZ|

## 返回码
|返回码|描述|
|---|---|
|**200**|OK|
