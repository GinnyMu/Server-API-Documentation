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



