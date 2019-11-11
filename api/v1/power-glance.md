# PowerGlance

## `/api/v1/power-app/power-glance/update`

更新 PowerGlance 数据.

### 请求参数

| 名称      | 类型             | 描述                      |
| --------- | ---------------- | ------------------------- |
| `token`   | `string`         | PowerGlance 授权 token    |
| `dataSet` | `DataSetEntry[]` | 新的 PowerGlance 统计数据 |

### 响应数据

`void`

## `/api/v1/power-app/power-glance/initialize`

初始化 PowerGlance 并获取全量资源数据.

### 请求参数

| 名称    | 类型     | 描述                   |
| ------- | -------- | ---------------------- |
| `token` | `string` | PowerGlance 授权 token |

### 响应数据

`InitializeResult | undefined`
