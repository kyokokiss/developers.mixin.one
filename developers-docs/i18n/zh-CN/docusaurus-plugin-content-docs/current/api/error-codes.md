---
title: 错误码
sidebar_position: 15
---

Mixin API 只会使用 20x 和 500，需要注意 500 错误，可能是 Web Server 而非 Mixin API Server 造成的。

| HTTP 状态码 | Mixin 错误码 | 描述                             |
| ----------- | ------------ | :------------------------------- |
| 202         | 400          | 请求正文无法作为有效数据进行解析 |
| 202         | 401          | 未经授权的访问                   |
| 202         | 403          | 禁止访问                         |
| 202         | 404          | 未找到 API 端点                  |
| 202         | 429          | 请求过多                         |
| 202         | 10006        | 需要更新 App                     |
| 202         | 20116        | 群聊已满                         |
| 202         | 20133        | 对话圈子太多                     |
| 500         | 500          | 内部服务器错误                   |
| 500         | 7000         | Blaze 服务器错误                 |
| 500         | 7001         | Blaze 操作超时                   |