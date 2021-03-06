
# 简洁版后台系统源码

## 开发框架操作说明

项目db脚本aylson_2018-04-08.sql.gz导入后默认的用户名和密码分别为superadmin/123456

1. 下载代码

2. 装好maven ,jdk工具

3. 复制aylson-manage/settings.xml到用户目录.m2下（利用国内阿里镜像，加速下载依赖包）

4. 进入项目目录aylson-manage，运行mvn jetty:run命令即可启动项目（默认访问地址：http://localhost:8080/manage/login.jsp）
（也可导入开发工具，然后进行相关jetty配置）

## 注意事项说明：

由于默认mysql导入文件大小有限制4m，而.sql导入文件很大，两种解决方式：
1. 修改mysql配置文件，调大导入文件限制（网上自查），使用show VARIABLES like '%max_allowed_packet%'，可查看默认最大大小（max_allowed_packet）
2. 不使用导入方式，而是直接复制.sql文件内容，然后粘贴到navicat工具查询中执行即可
3. 复制.sql内容时请注意：不要使用开发工具打开.sql文件，因为文件太大，文件内容显示不全，可使用editplus或者记事本工具打开即可


## [后台管理系统源码](https://github.com/hemin1003/aylson-parent)

基于SpringMVC4+EasyUI开发的[后台管理系统](https://github.com/hemin1003/aylson-parent)，已投入生产线上使用

体验系统地址：http://182.92.82.188:8280/manage/login.jsp

体验账号/密码，tmp1001/a123456

## 新增爬虫项目统计信息

爬虫信息框架，已实现抓取今日头条数据，测试数据每日均抓一万条左右

基于[JAVA爬虫框架实战](https://github.com/hemin1003/java-spider)实现

## 配套的前端API实现项目实战

基于SpringBoot实现的接口API系统，集成了拦截器，日志处理，mysql，mybatis, oauth2.0, spring secutity等功能，已投入生产线上使用

接口API系统源码：https://github.com/hemin1003/yfax-parent

## [关于我](http://heminit.com/about/)

欢迎交流问题，可加我的个人QQ 469580884，或群号 751925591，一起探讨交流问题

[我的博客地址](http://blog.csdn.net/hemin1003)

[个人域名](http://heminit.com)
