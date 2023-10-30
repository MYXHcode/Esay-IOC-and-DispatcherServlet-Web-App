# 简易的 IOC 和 DispatcherServlet Web 应用程序 project18-javaweb-book——尚硅谷学习笔记 2022 年

[TOC]

## 第 18 章 project18-javaweb-book 模块知识点

### 18.1 book 业务需求分析

### 18.2 数据库设计

1. 实体分析：

   - 图书 Book

   - 用户 User

   - 订单 Order

   - 订单详情 OrderItem

   - 购物车项 CartItem

2. 实体属性分析：

- 图书 : 书名、作者、价格、销量、库存、封面、状态。

- 用户 : 用户名、密码、邮箱。

- 订单 : 订单编号、订单日期、订单金额、订单数量、订单状态、用户。

- 订单详情 : 图书、数量、所属订单。

- 购物车项 : 图书、数量、所属用户。
