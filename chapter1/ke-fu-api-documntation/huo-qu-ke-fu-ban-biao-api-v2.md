## 获取客服班表API V2 {#获取客服班表api-v2}

| Tables | 说明 | 默认值 |
| :--- | :--- | :--- |
| URL | /api/v1/cs\_work |  |
| HTTP请求方式 | GET |  |
| 是否需要登录 | 否 |  |
| 授权访问限制 | 暂无 |  |
| 授权范围\(\) | 暂无 |  |
| 支持格式 | JSON |  |

表头参数:

| Tables | 类型及其范围 | 说明 | 默认值 |
| :--- | :--- | :--- | :--- |
| Authortoken | string | token验证信息 |  |

返回字段说明:

| Tables | 类型及其范围 | 说明 | 默认值 |
| :--- | :--- | :--- | :--- |
| ev\_result | number | 请求是否成功 | 0为成功, 1为错误 |
| ev\_message | string | 报错信息 | 空 |
| ev\_data | array | 客服班表信息 |  |

| ev\_data | 类型及其范围 | 说明 |
| :--- | :--- | :--- |
| id | number | 班表ID |
| uid | number | 客服ID |
| username | string | 客服名字 |
| valid\_from | string | 上班时间 |
| valid\_to | string | 下班时间 |
| zone | number | 工作区域 |

返回结果\(默认JSON\):

```
{
result :#0: successful 1:fail
message:
data:[
  {
   id: number,
   uid: number,
   username:string,
   valid_from: string,
   valid_to: string,
   zone:number
  }
 ]
}
```



