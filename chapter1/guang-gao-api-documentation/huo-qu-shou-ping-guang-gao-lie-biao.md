#### 获取首屏广告列表

| Tables | 说明 |
| :--- | :--- |
| URL |  |
| HTTP请求方式 | GET |
| 是否需要登录 | 需要 |
| 授权访问限制 | role 3 |
| 授权范围\(\) | 暂无 |
| 支持格式 | JSON |

表头参数:

| Tables | 类型及其范围 | 说明 |
| :--- | :--- | :--- |
| Authortoken | string | token验证信息 |

返回字段说明:

|  | 类型 | 说明 |
| :--- | :--- | :--- |
| result | number | 0为成功 1为失败 |
| ad\_launch | array | \[Object\] |

| \[ad\_launch object\] | 类型及其范围 | 说明 |
| :--- | :--- | :--- |
| id | number | 广告唯一id |
| navigation | string | 跳转链接地址 |
| status | 0 |  |
| avlb\_from | timestamp | 有效时间 |
| avlb\_to | timestamp | 结束时间 |
| image | string | 显示图片url |

返回结果\(默认JSON\):

```
{
    result: 0,
    ad_launch[
          {
            id:3,
            navigation:"",
            status:0,
            avlb_from:timestamp,
            avlb_to:timestamp,
  			image:"",
          }
        ]
}
```

  


