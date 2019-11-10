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

### 响应数据

`string` 访问令牌
