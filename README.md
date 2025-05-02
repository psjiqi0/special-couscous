# OpenWRT 常用指令脚本说明

本页整理了一些在 OpenWRT 上常用的操作指令，方便日常维护与调试使用。

---

## 📦 更新软件源

```sh
opkg update
```

---

## ⚙️ 修改 OpenWRT 页面端口

手动编辑配置文件：

```sh
vi /etc/config/uhttpd
```

---

## 🔁 重启 uhttpd 服务

```sh
/etc/init.d/uhttpd restart
```

---

## 🔥 重启防火墙

```sh
/etc/init.d/firewall restart
```

---

## 🧩 设置自定义 DNS 服务脚本

编辑启动脚本文件（自行添加内容）：

```sh
vi /etc/init.d/dns
```

添加完成后，设置开机启动并立即启动：

```sh
/etc/init.d/dns enable
/etc/init.d/dns start
```

---

## 🧪 测试 DDNS 临时进程运行

```sh
/tmp/ddns server --config /tmp/config.json
```

---

## 🧹 快速清理命令

删除临时文件与服务脚本：

```sh
rm /tmp/ddns
rm /tmp/cf.sh
rm /tmp/config.json
rm /etc/init.d/dns
```

结束相关进程（请将 `[PID]` 替换为实际进程号）：

```sh
kill -9 [PID]
```

---

> 📌 **注意：** 编辑文件、配置内容、脚本内容请根据具体需求修改，本 README 仅提供常用命令参考。
