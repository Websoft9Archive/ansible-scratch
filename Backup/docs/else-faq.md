# FAQ

#### Scratch support multi-language?

Yes, you can change language online

#### scratch-www project VS scratch-gui project?

[scratch-www](https://github.com/LLK/scratch-www)  = [scratch-gui](https://github.com/LLK/scratch-gui)  + Sharing community, Scratch-www user login function is still under development

#### Where is the database connection configuration of Scratch?

No need database now

#### If there is no domain name, can I deploy Scratch?

Yes, visit Scratch by *http://Internet IP*

#### Is it possible to modify the source path of Scratch?

Yes, modify it by [Nginx vhost configuration file](/stack-components.md)

#### How to change the permissions of filesytem?

Change owner(group) or permissions like below:

```shell
chown -R nginx.nginx /data/wwwroot
find /data/wwwroot -type d -exec chmod 750 {} \;
find /data/wwwroot -type f -exec chmod 640 {} \;
```
#### What's the difference between Deployment and Installation?

- Deployment is a process of installing and configuring a sequence of software in sequence in a different order, which is a complex system engineering.  
- Installation is the process of starting the initial wizard after the application is prepared.  
- Installation is simpler than deployment. 

#### What's Cloud Platform?

Cloud platform refers to platform manufacturers that provide cloud computing services, such as: **Azure, AWS, Alibaba Cloud, HUAWEI CLOUD, Tencent Cloud**, etc.

#### What is the difference between Instance, Cloud Server, Virtual Machine, ECS, EC2, CVM, and VM?

No difference, just the terminology used by different manufacturers, actually cloud servers