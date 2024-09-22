# Auth

用户接口

## 1. 登录

**Request**
```bash
POST {BASE_URL}/v1/token

{
  username: "john",
  password: "******"
}
```

**Response**

```json
{
  "code": "login-sucess",
  "message": "Login Successfully",
  "data": {
    "token": "AAAA.BBB.CCC"
  }
}
```

## 2. 用户信息

**Request**
```bash
GET {BASE_URL}/v1/me

Authorization: Bearer {JWT}
```

**Response**
```json
{
  "code": "user-profile",
  "message": "Get User Profile",
  "data": {
    "id": 1,
    "username": "jhon_doe",
    "display_name": "Jhon Doe",
    "balance": 123,
    "last_login": "2024-02-02 12:12:12",
    "history": { 
      "message": "最近玩过的游戏",
      "games": [
        {
          "id": 1,
          "name": "Slots"
        },
        {
          "id": 2,
          "name": "Slots 2"
        }
      ]
     }
  }
}
```


## PS: JWT Payload
JWT Payload 可以包含一些非敏感用户数据，方便后端针对用户身份做一些特殊处理。
比如 `{role: "admin"}`, 那后端可以直接知道这是一个来自 admin 的请求。

```json
{
  "user": {
    "id": 123,
    "roles": ["administrator"]
    ...
  }
}
```
