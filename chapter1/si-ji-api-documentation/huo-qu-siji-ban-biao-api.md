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



