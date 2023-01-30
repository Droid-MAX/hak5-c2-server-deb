hak5-c2-server-deb
===

[Hak5 Cloud C2 Basics](https://docs.hak5.org/cloud-c2/getting-started/cloud-c-basics)

**用法**

从发布页下载最新的软件包：[latest](https://github.com/Droid-MAX/hak5-c2-server-deb/releases/latest)

安装完毕后，根据实际情况修改配置文件，配置文件目录：`/etc/hak5/`，其中

`c2-base.cfg` 文件为默认基础配置文件

`c2-https.cfg` 为配置了自定义https证书时所使用的配置文件

`c2-proxy.cfg` 为配置了反向代理主机端口时所使用的配置文件

其中 `HOSTNAME` 参数为必填项

对应服务名称如下

`hak5-c2-server.service` - 使用基础配置文件 `c2-base.cfg` 启动C2服务

`hak5-c2-server-https.service` - 使用基础配置文件 `c2-base.cfg` 启动C2服务(HTTPS)

`hak5-c2-server-https-custom.service` - 使用自定义配置文件 `c2-https.cfg` 启动C2服务(HTTPS)

`hak5-c2-server-proxy.service` - 使用自定义配置文件 `c2-proxy.cfg` 启动C2服务
