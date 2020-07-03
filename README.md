# 定制 Docker 基础镜像

定制基础镜像，并上传到阿里云镜像仓库，以便于开发、部署使用。  
基于官方镜像源进行定制。

## node

基础镜像：node:14.4.0-alpine3.11  
定制修改：  
1.将 apk 镜像源更改为阿里云官方镜像站  
2.安装 gettext 包，以能够使用 envsubst 命令。  
镜像主页：https://cr.console.aliyun.com/repository/cn-shanghai/jian-public/node/details  
镜像版本：14.4.0-alpine3.11 (基础镜像), 14.4.0-alpine3.11-c (定制镜像)  
获取定制镜像：
```
docker pull registry.cn-shanghai.aliyuncs.com/jian-public/node:14.4.0-alpine3.11-c
```

## nginx

基础镜像：nginx:1.19.0-alpine  
定制修改：  
- 修改默认 nginx 设置，让 angular 路由功能能够正常工作。

镜像主页：https://cr.console.aliyun.com/repository/cn-shanghai/jian-public/nginx/details  
镜像版本：1.19.0-alpine (基础镜像), 1.19.0-alpine-c (定制镜像)   
获取定制镜像：
```
docker pull registry.cn-shanghai.aliyuncs.com/jian-public/nginx:1.19.0-alpine-c
```