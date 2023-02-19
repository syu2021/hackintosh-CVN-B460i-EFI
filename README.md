EFI请看Releases中介绍，适用于Ventura及以下任何macOS版本，网卡为AX200

配置一切完美，HDMI接口已定制（数据在下面图片或Releases），EFI未添加，请手动添加下

安装完系统请自行添加三码，USB有2个口为机箱（酷鱼T40）的，其他版本需要更换Wi-Fi和蓝牙驱动

下载地址：https://github.com/syu2021/hackintosh-CVN-B460i-EFI/releases

目前已知问题：睡眠唤醒后部分软件打开卡住

日志（时间从小到大）

1.beta4或其他版本睡眠问题或睡眠失败、关机不断电问题（与USB定制有关）修复方法

打开终端分别执行：

```
 pmset -g sched
 
 
 sudo pmset schedule cancelall
```

2.Ventura出现关机不断电可以通过强制关机后再开机再次关机解决

3.macOS Monterey 12.6或其他版本登陆不了Store请使用魔法

4.定制USB时发现主板右下角USB3.0可兼容2.0，有点奇怪，避免一些问题，直接删除了USB2.0端口（另附未修改前的USBkext）

5.解决睡眠唤醒后打开部分软件卡住问题

1.BIOS开启写保护

2.定制问题（在上面）

之后应该还会持续更新EFI,有问题请发到[syuyx@foxmail.com](mailto:syuyx@foxmail.com)或者GitHub的lssues里 最后感谢国光酱，AlphaGHX，乌龙蜜桃来一打，PCbeta和所有黑果大佬，祝你安装成功！