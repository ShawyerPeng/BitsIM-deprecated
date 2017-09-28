# 介绍
BitsIM，是一个移动即时通讯应用。

# 简述

# 目录结构

# 快速运行
前置条件：
* 安装 Mysql
* 安装 Maven

运行步骤：
* 创建数据库easyim, 并导入sql/easy_im_v1.sql
* 修改src/main/resources/applicationContext.xml中 mysql 的配置
* 在BitsIM-Server根目录执行maven jetty:run
* 使用 Post 请求localhost:8080/users/register确定服务是否正常启动

# 框架与技术
BitsIM Server 主要为 BitsIM 客户端提供 Restful API。主要使用了以下框架及第三方服务：
* Tomcat  运行的容器
* Spring 提供依赖注入
* SpringMVC 主要提供 Restful 支持
* MyBatis 数据库映射框架
* MySQL 存储用户信息，MongoDB 存储聊天信息
* Redis 热点数据缓存/提取
* RabbitMQ 消息发送队列
* Protobuf 序列化和反序列化
* MQTT 即时通讯协议
* Paho MQTT Client 实现
* Netty 网络框架
* 七牛云 用户发送的图片，语言存储服务
* JPush 提供最核心的消息推送支持

# API
