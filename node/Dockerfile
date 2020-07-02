FROM node:14.4.0-alpine3.11
WORKDIR /etc/apk
# 将 apk 镜像源替换为阿里云官方镜像站
COPY repositories .
# 安装 gettext 包，这样才能使用 envsubst 命令。
RUN apk add gettext