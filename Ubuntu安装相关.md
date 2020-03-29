### 1、安装独立显卡ubuntu启动黑屏
bios中设置中关闭集显。以技嘉主板为例：启动按del键进入bios==>集成外设==>内建显示设备=关闭。==>存储并离开。启动正常。    
![GigabyteBios](https://github.com/lix3972/hello-world/blob/master/pictures/GigabyteBiso.jpg)
### 2、用*.run安装
第一步：赋予.run文件的可执行权限(即x)

    r：读
    w：写
    x：执行

上面三者对应的值分别为4,2，1。因此赋予.run文件可执行权限可用命令：

sudo chmod 775 *.run
./*.run
