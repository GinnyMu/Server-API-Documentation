## 获取关店列表API {#商家关店管理----获取关店列表api}

| Tables | 说明 | 默认值 |
| :--- | :--- | :--- |
| URL | /api/v1/rr\_close |  |
| HTTP请求方式 | GET |  |
| 是否需要登录 | 否 |  |
| 授权访问限制 | 暂无 |  |
| 授权范围\(\) | 暂无 |  |
|  | 支持格式 | JSON |

表头参数:

| Tables | 类型及其范围 | 说明 | 默认值 |
| :--- | :--- | :--- | :--- |
|  | Authortoken | string | token验证信息 |

返回字段说明:\

| Table | 类型 | 说明 |
| :--- | :--- | :--- |
| ev\_result | string | 0为成功 1为失败 |
| ev\_message | string |  |
| ea\_data | array | array of restaurants |

| \[ev\_data\] | 类型及其范围 | 说明 | 默认值 |
| :--- | :--- | :--- | :--- |
| rid | string | 餐馆id |  |
| close\_id | string | 关店餐馆id |  |
| rr\_name | string | 餐馆名字 |  |
| start\_time | string | 开始关店时间 |  |
|  | end\_time | string | 结束关店时间 |

返回结果\(默认JSON\):

```
{
    ev_result: number,
    ev_message: string,
    ea_data:[
     {
     rid:"",
     id:"",
     name:"",
     start_time:"",
     end_time:""
     }
    ]
}
```



