#### 获取home广告列表

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
| ad\_home1 | array | \[Object\] 顶部banner |
| ad\_home2 | array | \[Object\] 下半部广告 |

| \[ad\_home1 ad\_home2 object\] | 类型及其范围 | 说明 |
| :--- | :--- | :--- |
| id | number | 广告唯一id |
| navitype | number | 1只显示图片不能点击 2跳转链接 3跳转商家 |
| nav\_url | string | 默认为空string，navitype2时有值 |
| image | string | 显示的图片url地址 |
| nav\_rid | number | 默认为空string，navitype3时有值 |
| sequence | number | 排序 |

返回结果\(默认JSON\):

```
{
    result: 0,
    ad_home1[
      {
        id:1,
        navitype:2,
  		nav_url:"",
  		image:"",
  		nav_rid:5,
  		sequence:2
      }
    ],
    ad_home2[
          {
            id:3,
            navitype:1,
            nav_url:"",
            image:"",
            nav_rid:3,
            sequence:4
          }
        ]
}
```





