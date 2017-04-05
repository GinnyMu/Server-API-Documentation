## 司机 API Documentation

* #### [`删除司机班表API`](#delete_driver_table)
* #### [`更新司机班表API`](#update_driver_table)
* #### [`添加司机班表API`](#add_driver_table)
* #### [`获取司机班表API`](#get_driver_table)

#### 

#### 删除司机班表API`PATCH /api/v1/dr_work`

* **Data Params**

  Authortoken

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

#### 更新司机班表API`PUT /api/v1/dr_work`

* **Data Params**

  Authortoken

  id

  driver\_id

  valid\_from

  valid\_to

  zone

  comment

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

#### 添加司机班表API`POST /api/v1/dr_work`

* **Data Params**

  Authortoken

  driver\_id

  valid\_from

  valid\_to

  zone

  comment

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

#### 获取司机班表API`GET /api/v1/dr_work`

* **Data Params**

  Authortoken

* **Return Params**

  ev\_result

  ev\_message

  ea\_data

* **Return Example**

```
{
ev_result :#0: successful 1:fail
ev_message:
ea_data:[
  {
   id: number,
   driver_id: number,
   wid:number,
   valid_from: string,
   valid_to: string,
   zone: number,
   comment: string
  }
 ]
}
```



