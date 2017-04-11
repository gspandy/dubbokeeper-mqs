# dubbokeeper-mqs

## dubbokeeper-mqs是什么

dubbokeeper-mqs是基于spring mvc开发的社区版dubboadmin集成服务管理以及服务监控一体的DUBBO服务管理系统，从[dubbokeeper](https://github.com/dubboclub/dubbokeeper)基础上整合而成的**MySQL快速启动版**，并新增服务预警接口、权限登录功能

dubbokeeper-mqs集成监控与展示，节省服务器资源，提供一键编译部署

## dubbokeeper-mqs包含哪些功能

- 应用管理
- 动态配置
- 统计信息
- Dubbo服务监控
- zookeeper信息查看
- 服务预警

---

执行数据库初始化脚本`application.sql`，数据库名可以自定义一个，编码采用utf-8

## 部署

只需配置`src/main/resources/dubbo.properties`与`pom.xml`的各属性值

打包部署到Tomcat启动

## 服务预警

修改`com.dubboclub.dk.alarm.impl.AlarmServiceImpl`的`void alarmHandle(URL url)`实现方法即可