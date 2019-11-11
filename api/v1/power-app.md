# PowerApp

## `/api/v1/power-app/publish`

发布 PowerApp.

### 权限

- `power-app:admin`

### 请求参数

| 名称         | 类型                     | 描述          |
| ------------ | ------------------------ | ------------- |
| `definition` | `PowerApp.RawDefinition` | PowerApp 定义 |

#### 示例数据

```json
{
  "definition": {
    "name": "hello-world",
    "displayName": "Hello World",
    "version": "0.1.0"
  }
}
```

### 响应数据

`string | undefined` 第一次发布时响应数据为用于确认来自 Makeflow 回调合法的令牌

#### 示例数据

```json
{
  "data": "72a41d5e-0828-4097-84d9-f4f13e799a5c"
}
```

## `/api/v1/power-app/refresh-token`

刷新 Makeflow 回调令牌.

### 权限

- `power-app:admin`

### 请求参数

| 名称   | 类型     | 描述            |
| ------ | -------- | --------------- |
| `name` | `string` | PowerApp `name` |

#### 示例数据

```json
{
  "name": "hello-world"
}
```

### 响应数据

`string` 新的回调令牌

#### 示例数据

```json
{
  "data": "8c31b9f3-f888-49d5-9bf3-040c74967c4a"
}
```
