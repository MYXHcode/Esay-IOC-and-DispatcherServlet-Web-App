# 简易的 IOC 和 DispatcherServlet Web 应用程序 project1-javaweb-begin——尚硅谷学习笔记 2022 年

[TOC]

## 第 1 章 project1-javaweb-begin 模块知识点

### 1.1 设置编码

#### 1.1.1 get 请求方式

```java
// get 方式在 Tomcat8 之后不需要设置编码
string name = request.getParameter("name");

// 1. 将字符串转换成字节数组
byte[] bytes = name.getBytes("ISO-8859-1");

// 2. 将字节数组按照设定的编码重新组装成字符串
name = new string(bytes,"UTF-8");
```

#### 1.1.2 post 请求方式

```java
// post 方式在 Tomcat10 之后不需要设置编码
request.setCharacterEncoding("UTF-8");
String name = request.getParameter("name");

```

> 注意: 设置编码必须在所有的获取参数动作之前。
