# FAQ

#### Scratch支持多语言吗？

支持多语言（包含中文），系统默认根据浏览器自动选择语言，并可以实时切换 

#### scratch-www 项目 和 scratch-gui 项目 有什么区别？

[scratch-www](https://github.com/LLK/scratch-www)  = [scratch-gui](https://github.com/LLK/scratch-gui)  + 分享社区，现在 scratch-www 用户登录功能还在开发中

#### 如果没有域名是否可以部署 Scratch？

可以，访问`http://服务器公网IP` 即可

#### 是否可以修改Scratch的源码路径？

可以，通过修改 [Nginx 虚拟主机配置文件](/zh/stack-components.md)中相关参数

#### 如何修改上传的文件权限?

```shell
chown -R nginx.nginx /data/wwwroot
find /data/wwwroot -type d -exec chmod 750 {} \;
find /data/wwwroot -type f -exec chmod 640 {} \;
```
#### 部署和安装有什么区别？

部署是将一序列软件按照不同顺序，先后安装并配置到服务器的过程，是一个复杂的系统工程。  
安装是将单一的软件拷贝到服务器之后，启动安装向导完成初始化配置的过程。  
安装相对于部署来说更简单一些。 

#### 云平台是什么意思？

云平台指提供云计算服务的平台厂家，例如：Azure,AWS,阿里云,华为云,腾讯云等

#### 实例，云服务器，虚拟机，ECS，EC2，CVM，VM有什么区别？

没有区别，只是不同厂家所采用的专业术语，实际上都是云服务器