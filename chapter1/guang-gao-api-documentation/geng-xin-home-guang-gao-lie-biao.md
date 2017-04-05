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

  ```
    result

    message
  ```

* **Return Example**

```
{    
      result:0,
      message:""
}
```



