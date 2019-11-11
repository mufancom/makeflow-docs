# 任务

## `/api/v1/task/create`

创建任务.

### 权限

- `task:create`

### 请求参数

| 名称          | 类型                               | 描述         |
| ------------- | ---------------------------------- | ------------ |
| `team`        | `string`                           | 团队 ID      |
| `procedure`   | `string`                           | 流程 ID      |
| `brief`       | `string`                           | 任务简述     |
| `description` | `string | undefined`               | 任务描述     |
| `tags`        | `string[] | undefined`             | 标签 ID 数组 |
| `assignee`    | `string | undefined`               | 任务负责人   |
| `outputs`     | `TaskPowerAppOutput[] | undefined` | 输出任务变量 |

### 响应数据

`string` 任务 ID

## `/api/v1/task/send-file-message`

发送文件消息.

### 权限

- `task:send-message`

### 请求参数

#### Query String 参数

| 名称       | 类型     | 描述           |
| ---------- | -------- | -------------- |
| `task`     | `string` | 任务 ID        |
| `fileName` | `string` | 文件名         |
| `type`     | `string` | 文件 MIME 类型 |

#### Body 参数

整个 Body 为上传的文件数据.

### 响应数据

`void`
