# 用户

## `/api/v1/user/match`

根据用户信息匹配用户.

### 权限

- `user:match`

### 请求参数

| 名称    | 类型     | 描述                   |
| ------- | -------- | ---------------------- |
| `email` | `string` | 用于匹配用户的邮箱地址 |

#### 示例数据

```json
{
  "email": "developer@makeflow.com"
}
```

### 响应数据

`string` 用户 ID

#### 示例数据

```json
{
  "data": "0b901806-5db3-4ee1-ad5c-9e89a47577ac"
}
```
