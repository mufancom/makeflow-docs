# Makeflow API v1

当前 API 处于测试阶段, 可能发生更改.

## 列表

- [account](account.md)
- [access-token](access-token.md)
- [user](user.md)
- [power-app](power-app.md)
- [power-glance](power-glance.md)
- [task](task.md)

## 约定

### 请求

如非特别说明, API 只接受 `application/json` 数据的 `POST` 请求.

### 响应

如非特别说明, API 响应为 `application/json` 数据.

- 当请求成功且返回值为 `undefined` 时, 响应数据为:

  ```json
  {}
  ```

  当请求成功且返回值不为 `undefined` 时, 响应数据为:

  ```json
  {
    "data": ...
  }
  ```

- 当请求失败时, 响应数据为:

  ```json
  {
    "error": {
      "code": "ERROR_CODE",
      "message": "Error message"
    }
  }
  ```

## 访问令牌权限

访问令牌可以通过不同的授权方式获取, 包括主动获取和被动获取 (PowerApp 授权).

| 权限名称     | 描述                     |
| ------------ | ------------------------ |
| `user:match` | 允许通过用户信息匹配用户 |
