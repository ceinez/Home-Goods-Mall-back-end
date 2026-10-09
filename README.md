# 家居商城后端（课程练习）

这是家居商城课程项目配套的 Koa 服务，用于向前端提供本地模拟数据和静态商品图片。项目用于学习简单路由、跨域配置和前后端联调，不是生产环境后端。

## 接口

| 方法 | 路径 | 说明 |
| --- | --- | --- |
| GET | `/goodscate` | 获取商品分类 |
| GET | `/goodslist/:cate_id` | 按分类获取商品列表 |
| GET | `/goods/:goods_id` | 获取商品详情 |
| GET | `/address/:user_id` | 获取模拟收货地址 |

商品图片等静态资源由 Koa 从 `static/` 目录提供。

## 课程背景与个人调整

这是课程引导下完成的商城后端练习。仓库提交记录显示，初始版本中补充了 Koa 服务、分类/商品/地址接口、配套本地数据和静态商品素材，用于与 Vue 前端联调。

## 技术栈

- Node.js
- Koa 2
- koa-router
- koa-static
- koa2-cors

## 本地运行

需要安装 Node.js 和 npm。在后端项目目录中运行：

```bash
npm install
node index.js
```

服务默认监听 `http://localhost:3000`。启动后可以访问 `http://localhost:3000/goodscate` 检查分类接口。

配套前端：[Home-Goods-Mall-front-end](https://github.com/ceinez/Home-Goods-Mall-front-end)

## 项目说明

当前仓库版本没有 MongoDB 或其他数据库的连接配置；接口数据由项目内的 JavaScript 文件返回。项目没有用户认证、真实支付或订单持久化，保留为课程学习记录，暂不持续维护。
