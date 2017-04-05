## 商家关店管理 API Documentation

* #### [`更新关店时间API`](#update_close_time)
* #### [`获取关店列表API`](#get_close_time)
* #### [`添加关店时间API`](#add_close_time)
* #### [`需求`](#require_close_time)
* #### [`rr_close_error`](#error_close_time)

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

  

#### 需求![](/assets/需求.jpg)



