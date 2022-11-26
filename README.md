# hackintosh-CVN-B460I-EFI
EFI请看Releases中介绍，适用于Ventura及以下任何macOS版本，网卡为AX200 

配置一切完美，HDMI接口已定制（数据在下面图片或Releases）

安装完系统请自行添加三码，USB有2个口为机箱（酷鱼T40）的，其他版本需要更换Wi-Fi和蓝牙驱动

下载地址：https://github.com/syu2021/hackintosh-CVN-B460i-EFI/releases

日志

1.beta4或其他版本睡眠问题或睡眠失败、关机不断电问题（与USB定制有关）修复方法

打开终端分别执行：


     pmset -g sched
     
     
     sudo pmset schedule cancelall


2.Ventura出现关机不断电可以通过强制关机后再开机再次关机解决    


3.macOS Monterey 12.6或其他版本登陆不了Store请使用魔法


4.定制USB时发现主板右下角USB3.0可兼容2.0，有点奇怪，避免一些问题，直接删除了USB2.0端口（另附未修改前的USBkext）     
     
之后应该还会持续更新EFI,有问题请发到syuyx@foxmail.com或者GitHub的lssues里
最后感谢国光酱，AlphaGHX，乌龙蜜桃来一打，PCbeta和所有黑果大佬，祝你安装成功！
![image](https://user-images.githubusercontent.com/88355063/204077857-e8dd2118-7b72-4ee9-beba-1783d30fe983.png)
![image](https://user-images.githubusercontent.com/88355063/181165444-c5226244-c94c-4ffc-aa9a-cb84eb1361fd.png)
![image](https://user-images.githubusercontent.com/88355063/181165449-30eb5938-999f-4fbe-9cf1-4bb40e5a4c41.png)
![image](https://user-images.githubusercontent.com/88355063/182870389-b6e135e5-2aa9-417b-b3b7-3f17852a5d2d.png)
