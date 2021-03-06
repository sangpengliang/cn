# revokePrivilege


## 描述
取消该账号对某个数据库的所有权限。权限取消后，该账号将不能访问此数据库。取消账号对某个数据库的访问权限，不影响该账号对其他数据库的访问权限

## 请求方式
POST

## 请求地址
https://rds.jdcloud-api.com/v1/regions/{regionId}/instances/{instanceId}/accounts/{accountName}:revokePrivilege

|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**regionId**|String|True| |地域代码，取值范围参见[《各地域及可用区对照表》](../Enum-Definitions/Regions-AZ.md)|
|**instanceId**|String|True| |RDS 实例ID，唯一标识一个RDS实例|
|**accountName**|String|True| |账号名，在同一个实例中账号名不能重复|

## 请求参数
|名称|类型|是否必需|默认值|描述|
|---|---|---|---|---|
|**dbNames**|String[]|True| |需要取消授权的数据库的名称。权限取消后，该账号将不能访问此数据库|


## 返回参数
无


## 返回码
|返回码|描述|
|---|---|
|**200**|OK|

## 请求示例
POST
```
public void testRevokePrivilege() {
    RevokePrivilegeRequest revokePrivilegeRequest = new RevokePrivilegeRequest();
    revokePrivilegeRequest.setAccountName("dj_ac");
    revokePrivilegeRequest.setInstanceId("mysql-wp4e9ztap2");
    revokePrivilegeRequest.setRegionId("cn-north-1");
    List<String> dbNames = new ArrayList<>();
    dbNames.add("dj_db");
    revokePrivilegeRequest.setDbNames(dbNames);
    RevokePrivilegeResponse response = rdsClient.revokePrivilege(revokePrivilegeRequest);
    System.out.println(new Gson().toJson(response));
}

```

## 返回示例
```
{
    "requestId": "bpa09sqv506u80guctqkucpwwi7g74q6"
}
```
