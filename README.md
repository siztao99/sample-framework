# API Framework - 使用说明

- 当前版本：1.0.0
- 发布日期：2015-10-25

[发布日志](RELEASE.md)

## 使用方法

### 第一步：构建 api-framework 模块

```
cd api-framework
mvn clean install
```

### 第二步：导入 SQL 脚本

```
cd sample-api
mysql -u root -p < doc/sql/schema.sql
```

### 第三步：启动 sample-api 应用（后端）

```
cd sample-api
mvn clean package tomcat7:run
```

### 第四步：启动 sample-web 应用（前端）

```
cd sample-web
mvn clean package tomcat7:run
```

### 第五步：访问应用程序

```
http://localhost:8082/
```


引用黄勇老师的 [从 MVC 到前后端分离](http://my.oschina.net/huangyong/blog/521891 "从 MVC 到前后端分离")
</br>
版权归黄勇老师所有[黄勇-博客](http://my.oschina.net/huangyong)