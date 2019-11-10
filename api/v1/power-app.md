# PowerApp

## `/api/v1/power-app/publish`

发布 PowerApp.

### 权限

- `power-app:admin`

### 请求参数

| 名称         | 类型                     | 描述          |
| ------------ | ------------------------ | ------------- |
| `definition` | `PowerApp.RawDefinition` | PowerApp 定义 |

### 响应数据

`string | undefined` 第一次发布时响应数据为用于确认来自 Makeflow 回调合法的令牌

## `/api/v1/power-app/refresh-token`

发布 PowerApp.

### 权限

- `power-app:admin`

### 请求参数

| 名称   | 类型     | 描述            |
| ------ | -------- | --------------- |
| `name` | `string` | PowerApp `name` |

### 响应数据

`string` 新的回调令牌
