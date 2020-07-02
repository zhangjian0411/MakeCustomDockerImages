# 定制 Docker 基础镜像

定制基础镜像，并上传到阿里云镜像仓库，以便于开发、部署使用。  
基于官方镜像源进行定制。

## node

基础镜像：node:14.4.0-alpine3.11  
定制修改：  
1.将 apk 镜像源更改为阿里云官方镜像站  
2.安装 gettext 包，以能够使用 envsubst 命令。  
镜像主页：https://cr.console.aliyun.com/repository/cn-shanghai/jian-public/node/details  
镜像版本：14.4.0-alpine3.11, 14.4.0-alpine3.11-c  
获取定制镜像：
```
docker pull registry.cn-shanghai.aliyuncs.com/jian-public/node:14.4.0-alpine3.11-c
```