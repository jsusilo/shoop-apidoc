1. Get product viewer
----------------------

- http://stage.api.getshoop.com/shoopv3/v3/product/viewer?id=4696&key=acf4effafa1bf7539d8e10eefddd419dbbb403a9
- http://api.getshoop.com/shoopv3/v3/product/viewer?id=4696&key=acf4effafa1bf7539d8e10eefddd419dbbb403a9

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

- http://stage.api.getshoop.com/shoopv3/v3/product/user-view?id=4696&key=acf4effafa1bf7539d8e10eefddd419dbbb403a9
- http://api.getshoop.com/shoopv3/v3/product/user-view?id=4696&key=acf4effafa1bf7539d8e10eefddd419dbbb403a9

Params:
- id = product id
- key = user key

Reponse:

```json
{"status":1}
```
