### **1.目前机子配置**

i9-10900TES（QTB0）

光威DDR4 白色马甲 3000Mhz 8GBx2

七彩虹B460i

致钛tiplus5000 512G

酷鱼T40

### **2.食用方法**

1.下载镜像和EFI:https://github.com/syu2021/hackintosh-CVN-B460i-EFI/releases 到U盘

使用TransMac或balenaEtcher制作镜像

2.BIOS设置

##### ①高级

CPU设置-C状态-**(关闭)**

CPU设置-cfg lock-**(关闭)**

SATA设置-SATA模式选择-**AHCI**

CSM配置-CSM support-**(关闭)**

##### ②主板芯片组

ME控制-**启动**

BIOS写保护-**开启**

**内存超频和唤醒可以自行设置**

### 3.USB定制

保留XHCI-unsupported.kext和开启XhciPortLimit，在hackintool定制，定制时要删除原有USBports，定制完关闭XhciPortLimit和添加USBports

### 4.EFI说明

基本完美，定制了HMDI接口，USB定制完成，OC版本和kext保持最新

出现WiFi和蓝牙问题请替换kext解决

替换网卡软件：ProperTree 、OpenCore Configurator 、OCAuxiliaryTools（个人推荐后两者）
WiFi：https://github.com/OpenIntelWireless/itlwm/releases

蓝牙：https://github.com/OpenIntelWireless/IntelBluetoothFirmware

蓝牙版本说明：big sur及以下使用IntelBluetoothInjector

Monterey及以上使用IntelBluetoothFirmware+BlueToolFixup+IntelBTPatcher

i5和i7设置imac20.1，i9设置20.2

![Xnip2023-02-19_23-43-59](/Users/syu/Desktop/Xnip2023-02-19_23-43-59.png)

![Xnip2023-02-19_23-43-13](/Users/syu/Desktop/Xnip2023-02-19_23-43-13.png)

![Xnip2023-02-19_23-43-42](/Users/syu/Desktop/Xnip2023-02-19_23-43-42.png)

![181165449-30eb5938-999f-4fbe-9cf1-4bb40e5a4c41](/Users/syu/Desktop/181165449-30eb5938-999f-4fbe-9cf1-4bb40e5a4c41.png)

![182870389-b6e135e5-2aa9-417b-b3b7-3f17852a5d2d](/Users/syu/Desktop/182870389-b6e135e5-2aa9-417b-b3b7-3f17852a5d2d.png)



### 日志（时间从小到大）

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

### 最后

之后应该还会持续更新EFI,有问题请发到[syuyx@foxmail.com](mailto:syuyx@foxmail.com)或者GitHub的lssues里 

最后感谢国光酱，AlphaGHX，乌龙蜜桃来一打，PCbeta和所有黑果大佬，祝你安装成功！

