# hackintosh-CVN-B460I-EFI
EFI的OC版本为0.85开发版，适用于Ventura beta6，网卡AX200，配置一切完美，HDMI接口已定制（数据在下面图片或Releases）

2022.10.2测试Ventura beta8Wi-Fi有问题，目前其他未测试，已替换EFI中Wi-Fi驱动使用macOS Monterey 12.6正常，登陆不了store请使用魔法

安装完系统请自行添加三码，USB有2个口为机箱（酷鱼T40）的，其他版本需要更换Wi-Fi和蓝牙驱动

下载地址：https://github.com/syu2021/hackintosh-CVN-B460i-EFI/releases

beta4睡眠问题或睡眠失败、关机不断电问题（与USB定制有关）修复方法

打开终端分别执行：  
     pmset -g sched    
     sudo pmset schedule cancelall

最新发现Ventura出现关机不断电可以通过强制关机后再开机再次关机解决
之后应该还会持续更新EFI,有问题请发到syuyx@foxmail.com或者GitHub的lssues里
最后感谢国光酱，AlphaGHX，乌龙蜜桃来一打，PCbeta和所有黑果大佬，祝你安装成功！
![image](https://user-images.githubusercontent.com/88355063/182590659-e492d306-4daa-412d-bce3-b8dafded9312.png)
![image](https://user-images.githubusercontent.com/88355063/181165444-c5226244-c94c-4ffc-aa9a-cb84eb1361fd.png)
![image](https://user-images.githubusercontent.com/88355063/181165449-30eb5938-999f-4fbe-9cf1-4bb40e5a4c41.png)
![image](https://user-images.githubusercontent.com/88355063/182870389-b6e135e5-2aa9-417b-b3b7-3f17852a5d2d.png)
