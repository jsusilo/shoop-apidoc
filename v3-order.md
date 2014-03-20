1. Find Order by User
----------------------


- http://stage.api.getshoop.com/shoopv3/v3/order/find-by-user?key=yourkey&limit=2&offset=0
- http://api.getshoop.com/shoopv3/v3/product/viewer?id=4696&key=yourkey

Params:

- key : user key
- limit
- offset

Response:

```json
{
  "status":1,
  "user_id":2831,
  "order_count":1,
  "orders":[{
      "id":2,
      "product": {
        "id":4329,
        "title":"tes",
        "currency":"IDR",
        "category":{
          "id":97,
          "name":"Others"
        },
        "user":{
          "id":667,
          "name":"Fahriyal Afif",
          "avatar":"2014-01-1390193388912.jpg"
        }
      },
      "quantity":1,
      "price":100,
      "address":"jalan semarang",
      "time":"2014-02-27 22:13:24"
    }
  ]
}
```
