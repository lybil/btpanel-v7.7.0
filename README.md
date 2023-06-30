# btpanel-v7.7.0
btpanel-v7.7.0-backup  官方原版v7.7.0版本面板备份

**Centos/Ubuntu/Debian安装命令 独立运行环境（py3.7）：**

```Bash
curl -sSO https://raw.githubusercontent.com/zhucaidan/btpanel-v7.7.0/main/install/install_panel.sh && bash install_panel.sh
```

跳过登录框，以及破解插件等请自行搜索

&nbsp;

**如果遇到重启后宝塔乱码 请DD最新版Debian系统然后修改语言区域：**


```Bash
nano /etc/default/locale
```

```Bash
LANG=en_US.UTF-8
```

修改后保存文件，重启VPS即可。

一个宝塔面板一键优化补丁，主要有以下优化项目：

1.去除宝塔面板强制绑定账号
2.去除各种删除操作时的计算题与延时等待
3.去除创建网站自动创建的垃圾文件（index.html、404.html、.htaccess）
4.关闭未绑定域名提示页面，防止有人访问未绑定域名直接看出来是用的宝塔面板
5.关闭活动推荐与在线客服
6.去除自动校验文件与上报信息定时任务

适用宝塔面板版本：7.7:

wget -O optimize.sh https://raw.githubusercontents.com/chenjinnian/bt_clean/master/optimize.sh && bash optimize.sh

适用宝塔面板7.9版本的命令（7.9版本不支持去除强制绑定账号，新增去除面板首页广告）：

wget -O optimize.sh https://raw.githubusercontents.com/chenjinnian/bt_clean/master/optimize_new.sh && bash optimize.sh

源码：https://github.com/chenjinnian/bt_clean
