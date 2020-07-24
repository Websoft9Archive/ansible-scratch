# Parameters

The Scratch deployment package contains a sequence software (referred to as "components") required for Scratch to run. The important information such as the component name, installation directory path, configuration file path, port, version, etc. are listed below.

## Path

### Scratch

Scratch project directory: */data/wwwroot/scratch*  
Scratch static web directory: */data/wwwroot/scratch/build*

> Scratch is based on Node.js, you can modify the source code and run build again

### Node.js

NPM directory: */usr/lib/node_modules/npm*  
Module global directory: */usr/lib/node_modules/npm/node_modules*   
Node bin directory: *usr/bin*

### Nginx

Nginx vhost configuration file: */etc/nginx/conf.d/default.conf*  
Nginx main configuration file: */etc/nginx/nginx.conf*  
Nginx logs file: */var/log/nginx/*

### MYSQL

No MySQL now


## Ports

These Ports is need when use Scratch, refer to [Safe Group Setting on Cloud Console](https://support.websoft9.com/docs/faq/tech-instance.html)

| Name | Number | Use |  Necessity |
| --- | --- | --- | --- |
| HTTP | 80 | HTTP requests for Scratch | Required |
| HTTPS | 443 | HTTPS requests Scratch | Optional |

## Version

You can see the version from product page of Marketplace. However, after being deployed to your server, the components will be automatically updated, resulting in a certain change in the version number. Therefore, the exact version number should be viewed by running the command on the server:

```shell
# Node.js Version
node --version

# Nginx version:
nginx -v
```