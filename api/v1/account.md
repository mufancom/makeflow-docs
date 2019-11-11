# 账号

## `/api/v1/account/list-users`

列出当前账号下的用户.

### 请求参数

| 名称       | 类型     | 描述         |
| ---------- | -------- | ------------ |
| `mobile`   | `string` | 用户手机号码 |
| `password` | `string` | 用户密码     |

#### 示例数据

```json
{
  "mobile": "18600000000",
  "password": "12345678"
}
```

### 响应数据

`UserCandidate[]` 用户列表

#### 示例数据

```json
{
  "data": [
    {
      "id": "5ac8ec44-30b6-4c08-bd43-cc811ed90045",
      "username": "vilic",
      "organization": {
        "id": "30b679a8-723e-4d67-a0e8-1d2ccba4b55f",
        "displayName": "Mufan"
      },
      "profile": {
        "fullName": "老万",
        "avatar": "https://foo/bar.jpg",
        "email": "foo@bar.com"
      }
    }
  ]
}
```
