## [广告API Documentation](#广告api-documentation)

* #### [`获取首屏广告列表`](#get-ad-launch)
* #### [`更新首屏广告列表`](#update-ad-launch)
* #### [`获取置顶商家列表`](#get-ad-rr)
* #### [`更新置顶商家列表`](#update-ad-rr)
* #### [`获取home广告列表`](#get-ad-home)
* #### [`更新home广告列表`](#update-ad-home)

## [司机 API Documentation](#driver-api)

* #### [`删除司机班表API`](#delete-driver-table)
* #### [`更新司机班表API`](#update-driver-table)
* #### [`添加司机班表API`](#add-driver-table)
* #### [`获取司机班表API`](#get-driver-table)

## [商家关店管理 API Documentation](#商家关店管理-api-documentation)

* #### [`更新关店时间API`](#update-close-time)
* #### [`获取关店列表API`](#get-close-time)
* #### [`添加关店时间API`](#add-close-time)
* #### [`需求`](#require-close-time)
* #### [`rr_close_error`](#error-close-time)

## [客服 API Documentation](#客服-api-documentation)

* #### [`删除客服班表`](#delete-service-table)
* #### [`更新客服班表`](#update-service-table)
* #### [`添加客服班表`](#add-service-table)
* #### [`获取客服名单`](#get-service-list)
* #### [`获取客服班表 V`](#get-service-table-v2)

##  

## 广告API Documentation {#ad-api}

#### [获取首屏广告列表](/chapter1/guang-gao-api-documentation/huo-qu-shou-ping-guang-gao-lie-biao.md)`GET mob/login` {#get-ad-launch}

* **Data Params**

  Authortoken

  result

  ad\_launch

* **Returns:**

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

#### 

#### [更新首屏广告列表](/chapter1/guang-gao-api-documentation/geng-xin-shou-ping-guang-gao-lie-biao.md)`POST url` {#update-ad-launch}

* **Data Params**

  Authortoken

  result

  ad\_launch

* **Data Example**

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

* **Return Params**

  result

  message

* **Returns Example:**

```
{    
      result:0,
      message:""
}
```

#### 

#### [获取置顶商家列表](/chapter1/guang-gao-api-documentation/huo-qu-zhi-ding-shang-jia-lie-biao.md)`GET url` {#get-ad-rr}

* **Data Params**

  Authortoken

* **Return Params**

  result

  ad\_rr

* **Return Example**

```
{
    result: 0,
    ad_rr[
      {
        zone:1,
        zone_description:"North Yorlk",
        adList:[
          {
            id:32,
            rid:56,
            zone:1,
            rank:4,
            start_date:timestamp,
            end_date:timestamp,
          }
        ]
      }
    ]
}
```

#### 

#### [更新置顶商家列表](/chapter1/guang-gao-api-documentation/geng-xin-zhi-ding-shang-jia-lie-biao.md)`POST url` {#update-ad-rr}

* **Data Params**

  Authortoken

  adList

* **Data Example**

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

* **Return Params**

  result

  message

* **Return Example**

```
{    
      result:0,
      message:""
}
```

#### 

#### [获取home广告列表](/chapter1/guang-gao-api-documentation/huo-qu-home-guang-gao-lie-biao.md)`GET url` {#get-ad-home}

* **Data Params**

  Authortoken

* **Return Params**

  result

  ad\_home1

  ad\_home2

* **Return Example**

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

#### 

#### [更新home广告列表](/chapter1/guang-gao-api-documentation/geng-xin-home-guang-gao-lie-biao.md)`POST url` {#update-ad-home}

* **Data Params**

  Authortoken

  ad\_home1

  ad\_home2

* **Data Example**

```
{
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

* **Return Params**

  result

  message

* **Return Example**

```
{    
      result:0,
      message:""
}
```

## 司机 API Documentation {#driver-api}

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

## 商家关店管理 API Documentation {#res-api}

#### 

#### [更新关店时间API](/chapter1/shang-jia-guan-dian-guanli-api-documentation/geng-xin-guan-dian-shi-jian-api.md)`PUT /api/v1/rr_close` {#update-close-time}

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

#### [获取关店列表API](/chapter1/shang-jia-guan-dian-guanli-api-documentation/huo-qu-guan-dian-lie-biao-api.md)`GET /api/v1/rr_close` {#get-close-time}

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

#### [添加关店时间API](/chapter1/shang-jia-guan-dian-guanli-api-documentation/tian-jia-guan-dian-shi-jian-api.md)`POST /api/v1/rr_close` {#add-close-time}

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

#### [需求![](/assets/需求.jpg)](/chapter1/shang-jia-guan-dian-guanli-api-documentation/xu-qiu.md) {#require-close-time}

#### [Restaurant Close Error Message](/chapter1/shang-jia-guan-dian-guanli-api-documentation/restaurant-close-error-message.md) {#error-close-time}

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

## 客服 API Documentation {#service-api}

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



