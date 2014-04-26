1. Check Phone Number Registered
---------------------------------

- http://stage.api.getshoop.com/shoopv3/v3/friend/check-phone-number-registered
- http://api.getshoop.com/shoopv3/v3/friend/check-phone-number-registered

POST Params:
- key = yourkey
- phone_numbers = phonenumber1,phonumber2,phonumber3

Response:

```json
{
    "status": 1,
    "users": [
        {
            "id": 2,
            "name": "bane",
            "phone": "1234",
            "avatar": null,
            "follow_status": 0,
            "product_count": "1"
        },
    ]
}
```
