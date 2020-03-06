### 1. /usr/lib/xorg/Xorg --未验证
参考：https://forum.ubuntu.org.cn/viewtopic.php?t=134968  
这个是firefox的问题。
因为FF缓存了大量的网页内容，来报告安全威胁。
而导致了频繁的IO读取。  
解决办法：  
缓存文件是~/.mozilla/firefox/xxxxx.default/下的urlclassifier*.sqlite
Edit->Preferences->Security，去掉Tell me if the site...那两项.
然后删除缓存文件urlclassifier*.sqlite  
重启Xwidow，重启firefox。
### 2. compiz 
桌面特效 相关进程  
关闭方法：参考https://blog.csdn.net/jiankunking/article/details/69467757  
(1)下载安装CompizConfig设置管理器   
(2)禁用下面这几个项:Enhanced Zoom Desktop, Animations, Fading Windows, Window Decoration   
版本不同选项可能有所变化。
