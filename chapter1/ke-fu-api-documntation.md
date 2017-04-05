## 客服 API Documntation

* #### [`删除客服班表`](#delete-service-table)
* #### [`更新客服班表`](#update-service-table)
* #### [`添加客服班表`](#add-service-table)
* #### [`获取客服名单`](#get-service-list)
* #### [`获取客服班表 V2`](#get-service-table-v2)

####            

#### [删除客服班表API](/chapter1/ke-fu-api-documntation/shan-chu-ke-fu-ban-biao-api.md)`PATCH /api/v1/cs_work` {#delete-service-table}

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

#### [更新客服班表API](/chapter1/ke-fu-api-documntation/geng-xin-ke-fu-ban-biao-api.md)`PUT /api/v1/cs_work` {#update-service-table}

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

#### [添加客服班表API](/chapter1/ke-fu-api-documntation/tian-jia-ke-fu-ban-biao-api.md)`POST /api/v1/cs_work` {#add-service-table}

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

#### [获取客服名单API](/chapter1/ke-fu-api-documntation/huo-qu-ke-fu-ming-dan.md)`GET /api/v1/cs_role` {#get-service-list}

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

####             

#### [获取客服班表API V2](/chapter1/ke-fu-api-documntation/huo-qu-ke-fu-ban-biao-api-v2.md)`GET /api/v1/cs_work` {#get-service-table-v2}

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



