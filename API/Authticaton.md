# Auth

# login

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
  code: "login-sucess",
  message: "Login Successfully",
  data: {
    token: "AAAA.BBB.CCC"
  }
}
```
