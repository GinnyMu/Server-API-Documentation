## 更新司机班表API {#更新客服班表api}

| Tables | 说明 | 默认值 |
| :--- | :--- | :--- |
| URL | /api/v1/dr\_work |  |
| HTTP请求方式 | PUT |  |
| 是否需要登录 | 否 |  |
| 授权访问限制 | 暂无 |  |
| 授权范围\(\) | 暂无 |  |
| 支持格式 | JSON |  |

表头参数:

| Tables | 类型及其范围 | 说明 | 默认值 |
| :--- | :--- | :--- | :--- |
| Authortoken | string | token验证信息 |  |

请求参数:

| Tables | 类型及其范围 | 说明 | 默认值 |
| :--- | :--- | :--- | :--- |
| id | number | 班表ID |  |
| driver\_id | number | 客服ID |  |
| valid\_from | string | 上班时间 |  |
| valid\_to | string | 下班时间 |  |
| zone | number | 工作区域 |  |
| comment | string | 备注 |  |

返回字段说明:

| Tables | 类型及其范围 | 说明 | 默认值 |
| :--- | :--- | :--- | :--- |
| ev\_result | number | 请求是否成功 | 0为成功, 1为错误 |
| ev\_message | string | 报错信息 | 空 |

返回结果\(默认JSON\):

```
{
    ev_result: number,
    ev_message: string
}
```



