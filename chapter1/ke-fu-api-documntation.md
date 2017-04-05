## 客服 API Documntation

* #### [`删除客服班表`](#delete_service_table)
* #### [`更新客服班表`](#update_service_table)
* #### [`添加客服班表`](#add_service_table)
* #### [`获取客服名单`](#get_service_list)
* #### [`获取客服班表 V2`](#get_service_table_v2)

#### 

#### 删除客服班表API`PATCH /api/v1/cs_work`

* **Data Params**

  Authortoken

  id

* **Return Params**

  ev\_result

  ev\_message

* **Return Example**

```
{
    result: number,
    message: string
}
```

####   

#### 更新客服班表API`PUT /api/v1/cs_work`

* **Data Params**

  Authortoken

  id

  uid

  valid\_from

  valid\_to

  zone

* **Return Params**

  ev\_result

  ev\_message

* **Return Example**

```
{
    result: number,
    message: string
}
```

####   

#### 添加客服班表API`POST /api/v1/cs_work`

* **Data Params**

  Authortoken

  uid

  valid\_from

  valid\_to

  zone

* **Return Params**

  ev\_result

  ev\_message

* **Return Example**

```
{
    result: number,
    message: string
}
```

####   

#### 获取客服名单API`GET /api/v1/cs_role`

* **Data Params**

  Authortoken

* **Return Params**

  ev\_result

  ev\_message

  ev\_data

* **Return Example**

```
result :#0: successful 1:fail
message:
data:[
  {
    uid: number,
    username: string
  }
]
```

  

#### 获取客服班表API V2`GET /api/v1/cs_work`

* **Data Params**

  Authortoken

* **Return Params**

  ev\_result

  ev\_message

  ev\_data

* **Return Example**

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



