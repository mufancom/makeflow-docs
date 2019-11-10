# 账号

## `/api/v1/account/list-users`

列出当前账号下的用户.

### 请求参数

| 名称       | 类型     | 描述         |
| ---------- | -------- | ------------ |
| `mobile`   | `string` | 用户手机号码 |
| `password` | `string` | 用户密码     |

### 响应数据

`UserCandidate[]` 用户列表
