# Gin_demoTo_FC
部署一个 gin web 框架项目到阿里云函数计算 FC 中

查看效果：http://gin-web-demo-mph1-devs.learning-6-6.1581223139287319.cn-shenzhen.fc.devsapp.net/

### 本项目目录

- src                                     Gin应用示例源码
- gin_devs_mph                 使用Devs工具部署目录
- gin_console_mph            使用控制台手动部署目录

### Devs工具一键部署

> 前提是已安装好 serverless devs 工具并已经配置好个人账号密钥

进入到 gin_devs_mph 项目目录，在命令行执行

```shell
s deploy
```

### 控制台手动部署

在阿里云 FC 控制台创建函数选择 custom runtime 然后上传 zip 包，即gin_console_mph 项目目录中的 `go-gin.zip`，然后设置启动命令为

```shell
./main
```

