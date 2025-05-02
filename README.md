Copy
## 更新软件包

更新软件包可以查看架构核心。

```bash
opkg update
修改OpenWrt页面端口
修改OpenWrt页面端口。

Copy
vi /etc/config/uhttpd
重启uhttpd
重启uhttpd。

Copy
/etc/init.d/uhttpd restart
重启防火墙
重启防火墙。

Copy
/etc/init.d/firewall restart
编辑DNS文件
编辑DNS文件。

Copy
vi /etc/init.d/dns
重启init.d
重启init.d。

Copy
/etc/init.d/dns enable
/etc/init.d/dns start
测试进程
测试进程是否正常。

Copy
/tmp/ddns server --config /tmp/config.json
快速删除命令
快速删除命令。

Copy
rm /tmp/ddns
rm /tmp/cf.sh
rm /tmp/config.json
rm /etc/init.d/dns
kill -9 进程号
Copy
这样，当你复制代码块时，只会复制代码本身，而不会包含中文说明文字。将上述内容保存到你的READM
