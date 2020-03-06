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
