# 访问令牌

## `/api/v1/access-token/create`

创建访问令牌.

### 请求参数

| 名称          | 类型       | 描述           |
| ------------- | ---------- | -------------- |
| `mobile`      | `string`   | 用户手机号码   |
| `password`    | `string`   | 用户密码       |
| `user`        | `string`   | 用户 ID        |
| `permissions` | `string[]` | 请求的权限列表 |

> 目前可以通过此 API 获取的权限只有 `power-app:admin`.

#### 示例数据

```json
{
  "mobile": "18600000000",
  "password": "12345678",
  "user": "5ac8ec44-30b6-4c08-bd43-cc811ed90045",
  "permissions": ["power-app:admin"]
}
```

### 响应数据

`string` 访问令牌

#### 示例数据

```json
{
  "data": "e8ee5b2a-a717-4f46-8908-b07e208c3b2e"
}
```
