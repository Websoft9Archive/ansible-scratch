# 初始化安装

在云服务器上部署 Scratch 预装包之后，请参考下面的步骤快速入门。

## 准备

1. 在云控制台获取您的 **服务器公网IP地址** 
2. 在云控制台安全组中，检查 **Inbound（入）规则** 下的 **TCP:80** 端口是否开启
3. 若想用域名访问 Scratch，请先到 **域名控制台** 完成一个域名解析

## Scratch 安装向导

1. 使用本地电脑的 Chrome 或 Firefox 浏览器访问网址：*http://域名* 或 *http://Internet IP*, 就进入了Scratch
![Scratch初始化页面](https://libs.websoft9.com/Websoft9/DocsPicture/zh/scratch/scratch-gui-websoft9.png)

2. Scratch首次加载数据超过20M，如果您的网络带宽不足的话，加载会很慢，耐心等待

> 需要了解更多Scratch的使用，请参考官方文档：[Scratch Documentation](https://en.scratch-wiki.info)

## 常见问题

#### 浏览器打开IP地址，无法访问 Scratch（白屏没有结果）？

您的服务器对应的安全组80端口没有开启（入规则），导致浏览器无法访问到服务器的任何内容

#### Scratch打开很慢？

Scratch首次加载数据超过20M。例如：您使用的是2M带宽，那么理想情况下的加载时间为：2000k/(128k/s×2)=7.8s。显然，如果带宽不足，速度会非常慢。
