# API 概述

这是 API 文档的示例页面。

## 示例 API

### GET /api/users

获取用户列表

**响应**

```json
{
  "code": 200,
  "data": [
    { "id": 1, "name": "张三" },
    { "id": 2, "name": "李四" }
  ]
}
```

### POST /api/users

创建新用户

**请求体**

```json
{
  "name": "王五",
  "email": "wangwu@example.com"
}
```

**响应**

```json
{
  "code": 201,
  "data": {
    "id": 3,
    "name": "王五",
    "email": "wangwu@example.com"
  }
}
```

## 代码示例

::: tip 提示
使用代码块展示示例代码
:::

```javascript
// JavaScript 示例
async function fetchUsers() {
  const response = await fetch('/api/users')
  const data = await response.json()
  return data
}
```

```python
# Python 示例
import requests

def fetch_users():
    response = requests.get('/api/users')
    return response.json()
```

## 表格示例

| 参数 | 类型 | 必填 | 描述 |
|------|------|------|------|
| id | number | 是 | 用户 ID |
| name | string | 是 | 用户名称 |
| email | string | 否 | 邮箱地址 |
