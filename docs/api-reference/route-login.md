# API route: /login

## POST method
Login a user

### Parameters
```json
{
  "username": "onmyshelf",
  "password": "passwordEncodedInBase64"
}
```

### Return example
```json
{
  "token": "dcb1b2b20707a060e72ba8013ac5",
  "userid": 1,
  "readonly": false
}
```
