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

4. Get product lover
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

5. Update Stock
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
