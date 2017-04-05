## 广告API Documentation

* #### `获取首屏广告列表`
* #### [`更新首屏广告列表`](/chapter1/guang-gao-api-documentation/geng-xin-shou-ping-guang-gao-lie-biao.md)
* #### [`获取置顶商家列表`](#get_ad_rr)
* #### [`更新置顶商家列表`](#update_ad_rr)
* #### [`获取home广告列表`](#get_ad_home)
* #### [`更新home广告列表`](#update_ad_home)

#### 

#### 获取首屏广告列表`GET mob/login`

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

#### 更新首屏广告列表`POSTurl`

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

#### 获取置顶商家列表`GET url`

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

#### 更新置顶商家列表`POST url`

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

#### 获取home广告列表`GET url`

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

#### 更新home广告列表`POST url`

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



