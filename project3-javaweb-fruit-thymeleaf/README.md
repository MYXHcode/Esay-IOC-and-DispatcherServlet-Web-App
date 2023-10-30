# 简易的 IOC 和 DispatcherServlet Web 应用程序 project3-javaweb-fruit-thymeleaf——尚硅谷学习笔记 2022 年

[TOC]

## 第 3 章 project3-javaweb-fruit-thymeleaf 模块知识点

### 3.1 Thymeleaf 视图模板技术

#### 3.1.1 开发步骤

1. 添加 Thymeleaf 的 jar 包。

2. 新建一个 Servlet 类 ViewBaseServlet。

3. 在 web.xml 文件中添加配置。

   - 配置前缀：view-prefix

   - 配置后缀：view-suffix

4. 使 Servlet 继承 ViewBaseServlet。

5. 根据逻辑视图名称，得到物理视图名称。

   - 此处的视图名称是 index。

   - 那么 Thymeleaf 会将这个逻辑视图名称对应到物理视图名称上去。

   - 逻辑视图名称：index

   - 物理视图名称：view-prefix + 逻辑视图名称 + view-suffix

   - 所以真实的视图名称是：/index.html

   ```java
       super.processTemplate("index",request,response);
   ```

6. 使用 Thymeleaf 的标签。
   - th:if
   - th:unless
   - th:each
   - th:text
