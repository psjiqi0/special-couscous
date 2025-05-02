```python
def hello_world():
    print("opkg update")

opkg update
更新软件软可以看架构核心
vi /etc/config/uhttpd
修改openwrt页面端口
/etc/init.d/uhttpd restart
重启uhttpd
/etc/init.d/firewall restart   #防火墙

vi /etc/init.d/dns
文件dns
重启init.d
/etc/init.d/dns enable
/etc/init.d/dns start
/tmp/ddns server --config /tmp/config.json   #测试进程正常
#快速删除命令
rm /tmp/ddns
rm /tmp/cf.sh
rm /tmp/config.json
rm /etc/init.d/dns
kill -9 进程号

