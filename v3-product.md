1. Get product viewer
----------------------

- http://stage.api.getshoop.com/shoopv3/v3/product/viewer?id=4696&key=yourkey
- http://api.getshoop.com/shoopv3/v3/product/viewer?id=4696&key=yourkey

Params:
- id = product id

Response:

```json
{
  "view_count":4,
  "viewed_by":  [
    {"id":2880,"name":"andyajadeh7", "following": 0},
    {"id":2831,"name":"andyshoop", "following": 1}
  ]
}
```

2. Catat View Product
----------------------

- http://stage.api.getshoop.com/shoopv3/v3/product/user-view?id=4696&key=yourkey
- http://api.getshoop.com/shoopv3/v3/product/user-view?id=4696&key=yourkey

Params:
- id = product id
- key = user key

Reponse:

```json
{"status":1}
```

3. Post comment
----------------

- http://stage.api.getshoop.com/shoopv3/v3/product/post-comment?id=4696&key=yourkey&comment=thecomment
- http://api.getshoop.com/shoopv3/v3/product/post-comment?id=4696&key=yourkey&comment=thecomment

Params:
- id = product id
- key = user key
- comment = the comment text

Reponse:

```json
{"status":1}
```

4. Get product comment
-----------------------

- http://stage.api.getshoop.com/shoopv3/v3/product/comment?id=4696&key=yourkey&limit=5&before-comment-id=2
- http://api.getshoop.com/shoopv3/v3/product/comment?id=4696&key=yourkey&limit=5&before-comment-id=2

Params:
- id = product id
- before-comment-id = before comment id

Response:

```json
{"status":1,"product_id":4696,"comment_count":4,"comments":[{"id":3,"user":{"name":"andyshoop","avatar":null},"time":"2014-03-17 15:12:39","comment":"haha"},{"id":4,"user":{"name":"andyshoop","avatar":null},"time":"2014-03-17 15:17:08","comment":"haha"}]}
```

5. Get product lover
----------------------

- http://stage.api.getshoop.com/shoopv3/v3/product/lover?id=4696&key=yourkey
- http://api.getshoop.com/shoopv3/v3/product/lover?id=4696&key=yourkey

Params:
- id = product id

Response:

```json
{
  "love_count":4,
  "loved_by":  [
    {"id":2880,"name":"andyajadeh7", "following": 0, "avatar": null},
    {"id":2831,"name":"andyshoop", "following": 1, "avatar": null}
  ]
}
```

6. Update Stock
----------------

- http://stage.api.getshoop.com/shoopv3/v3/product/update-stock?id=4696&key=yourkey
- http://api.getshoop.com/shoopv3/v3/product/update-stock?id=4696&key=yourkey

GET Params:
- id = product id
- key

POST Params:
- stock = stock to update (integer)

Response:

```json
{
  "status":1
}
```

7. Product Detail
------------------

- http://stage.api.getshoop.com/shoopv3/v3/product/detail?id=4692&key=yourkey
- http://api.getshoop.com/shoopv3/v3/product/detail?id=4692&key=yourkey

GET Params:
- id = product id
- key = user key

Response:

```json
{
  "status":1,
  "product":{
    "id":4692,
    "title":"Hobo bag nih",
    "desc":"hobo bag nih, mau?",
    "price":2750000,
    "currency":"IDR",
    "how_to_order":null,
    "status":0,
    "share":null,
    "image":null,
    "tag":null,
    "stock":null,
    "langitude":null,
    "longitude":null,
    "time":"2014-03-12 19:23:27",
    "id_user":2880,
    "fb_post":null,
    "hubmeup_link":null,
    "from_app":null,
    "id_supercat":null,
    "id_buyercat":61,
    "id_superloc":null,
    "discount":null,
    "view_count":12,
    "shoop_count":4,
    "comment_count":6,
    "is_nego":false,
    "image_migrate":true,
    "condition":"New",
    "supercat":null,
    "buyercat":{
      "id":61,
      "name":"Hobo Bag"
    },
    "superloc":null,
    "images":[{
        "id":1834,
        "image":"bdfe435740d2ec936195ea399923214d.png"
      },{
        "id":1835,
        "image":"7f11f8e4bc0469b5b0db8602a4529658.png"
      },{
        "id":1836,
        "image":"f820ca1aad95bcc28a1ca35976009a65.png"
      },{
        "id":1837,
        "image":"222cde83c2eb2696f6129081da1525ff.png"
      }
    ],
    "tags":[],
    "link":[],
    "user":{
      "id":2880,
      "name":"andyajadeh7",
      "email":"andyajadeh7@gmail.com",
      "phone":"08132328832",
      "address":null,
      "city":null,
      "country":null,
      "avatar":null,
      "location":null,
      "follow":{
        "following":0,
        "follower":1
      },
      "product_count":{
        "all":2
      }
    }
  }
}
```

8. Post share
--------------

- http://stage.api.getshoop.com/shoopv3/v3/product/post-share
- http://api.getshoop.com/shoopv3/v3/product/post-share

POST Params:
- id = product id
- key = user key
- to-facebook = 0|1
- to-twitter  = 0|1

Reponse:

```json
{
    "status": 1,
    "share": {
        "id": 4,
        "user": {
            "id": 2831,
            "name": "andyshoop",
            "avatar": null
        },
        "time": "2014-03-23 13:48:29",
        "facebook_url": null,
        "twitter_url": null
    }
}
```
