# Auth

## login

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

## JWT Payload
JWT Payload 可以包含一些非敏感用户数据，方便后端针对用户身份做一些特殊处理。
比如 `{role: "admin"}`, 那后端可以直接知道这是一个来自 admin 的请求。

```json
{
  "user": {
    "id": 123,
    ...
  }
}
```
