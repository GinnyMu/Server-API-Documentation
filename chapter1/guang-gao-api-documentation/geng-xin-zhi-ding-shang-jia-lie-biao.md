#### 更新置顶商家列表

| Tables | 说明 |
| :--- | :--- |
| URL |  |
| HTTP请求方式 | POST |
| 是否需要登录 | 需要 |
| 授权访问限制 | role 3 |
| 授权范围\(\) | 暂无 |
| 支持格式 | JSON |

表头参数:

| Tables | 类型及其范围 | 说明 |
| :--- | :--- | :--- |
| Authortoken | string | token验证信息 |

请求字段说明:

|  | 类型 | 说明 |
| :--- | :--- | :--- |
| adList | array | \[Object\] |

| \[adList object\] | 类型及其范围 | 说明 |
| :--- | :--- | :--- |
| id | number | 广告id 唯一 |
| rid | number | 餐馆rid |
| zone | number | 区域id |
| rank | number | 排序，越大越靠前 |
| start\_date | timestamp | 起始日期 |
| end\_date | timestamp | 结束 |
| status | number | 0/1 1为删除 |



请求参数\(默认JSON\):

```
{	
  	adList:[
          {
            id:32,
            rid:56,
            zone:1,
			rank:4,
            start_date:timestamp,
            end_date:timestamp,
  			status:1
          }
        ]
}
```

返回字段说明:

|  | 类型 | 说明 |
| :--- | :--- | :--- |
| result | number | 0成功 1 失败 |
| message | string | 报错信息 |

返回参数\(默认JSON\):

```
{	
  	result:0,
  	message:""
}
```



