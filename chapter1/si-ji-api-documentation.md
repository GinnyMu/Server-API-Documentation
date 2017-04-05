## 司机 API Documentation

* #### [`删除司机班表API`](#delete-driver-table)
* #### [`更新司机班表API`](#update-driver-table)
* #### [`添加司机班表API`](#add-driver-table)
* #### [`获取司机班表API`](#get-driver-table)

####           

#### [删除司机班表API](/chapter1/si-ji-api-documentation/shan-chu-si-ji-ban-biao-api.md)`PATCH /api/v1/dr_work` {#delete-driver-table}

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

#### [更新司机班表API](/chapter1/si-ji-api-documentation/geng-xin-si-ji-ban-biao-ap.md)`PUT /api/v1/dr_work` {#update-driver-table}

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

#### [添加司机班表API](/chapter1/si-ji-api-documentation/tian-jia-si-ji-ban-biao-api.md)`POST /api/v1/dr_work` {#add-driver-table}

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

#### [获取司机班表API](/chapter1/si-ji-api-documentation/huo-qu-siji-ban-biao-api.md)`GET /api/v1/dr_work` {#get-driver-table}

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



