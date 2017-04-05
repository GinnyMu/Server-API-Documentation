## 商家关店管理 API Documentation

* #### [`更新关店时间API`](#update_close_time)
* #### [`获取关店列表API`](#get_close_time)
* #### [`添加关店时间API`](#add_close_time)
* #### [`需求`](#require_close_time)
* #### [`rr_close_error`](#error_close_time)

####   

#### 更新关店时间API`PUT /api/v1/rr_close`

* **Data Params**

  Authorken

  rid

  start\_time

  end\_time

  id

* **Return Params**

  ev\_result

  ev\_message

* **Return Example**

```
{
    ev_result: number,
    ev_message: string
}
```

####   

#### 获取关店列表API`GET /api/v1/rr_close`

* **Data Params**

  Authortoken

* **Return Params**

  ev\_result

  ev\_message

  ea\_data

* **Return Example**

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

####   

#### 添加关店时间API`POST /api/v1/rr_close`

* **Data Params**

  Authortoken

  rid

  start\_time

  end\_time

* **Return Params**

  ev\_result

  ev\_message

* **Return Example**

```
{
    ev_result: number,
    ev_message: string
}
```

####   

#### 需求![](/assets/需求.jpg)

#### Restaurant Close Error Message

`GET, PUT, POST`

`http://test.norgta.com/public/api/v1/rr_close`

* **报错信息:**

| Error Code | Error Message | Description |
| :--- | :--- | :--- |
| 70001 | Authrorization Failed: invalid token | Token验证不通过 |
| 70002 | Cannot find header: Authortoken | Header找不到'Authortoken' |
| 70003 | Number of Invalid amount of arguments | 给予参数数量不符合 |
| 70004 | Authorization Failed: Permission denied | 此用户不是管理员 |
| 70005 | Authorization Failed: unrecognized user | 没有此用户 |



