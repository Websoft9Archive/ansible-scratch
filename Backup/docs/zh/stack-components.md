# 参数

Scratch 预装包包含 Scratch 运行所需一序列支撑软件（简称为“组件”），下面列出主要组件名称、安装路径、配置文件地址、端口、版本等重要的信息。

## 路径

### Scratch

Scratch 项目目录： */data/wwwroot/scratch-gui*  
Scratch 静态页面目录： */data/wwwroot/scratch-gui/build*  

> Scratch 基于Node开发，可以通过修改Node.js后再次构建发布

### Node.js

NPM 路径: */usr/lib/node_modules/npm*  
Module 全局路径：*/usr/lib/node_modules/npm/node_modules*
Node 可执行文件路径：*usr/bin*

### Nginx

Nginx 虚拟主机配置文件：*/etc/nginx/conf.d/default.conf*  
Nginx 主配置文件： */etc/nginx/nginx.conf*  
Nginx 日志文件： */var/log/nginx/*

### MYSQL

暂无数据库

## 端口号

下面是您在使用本镜像过程中，需要用到的端口号，请通过 [云控制台安全组](https://support.websoft9.com/docs/faq/zh/tech-instance.html)进行设置

| 名称 | 端口号 | 用途 |  必要性 |
| --- | --- | --- | --- |
| HTTP | 80 | 通过http访问Scratch | 必须 |
| HTTPS | 443 | 通过https访问Scratch | 可选 |

## 版本号

组件版本号可以通过云市场商品页面查看。但部署到您的服务器之后，组件会自动进行更新导致版本号有一定的变化，故精准的版本号请通过在服务器上运行命令查看：

```shell
# Node.js Version
node --version

# Nginx version:
nginx -v

```