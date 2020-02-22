# 第八课 root教程(第三方root工具)
* 下载安装 [TWRP](https://twrp.me/Devices/)  与TWRP.img(版本要一致)这里是[google](https://twrp.me/Devices/Google/)

* 下载安装[su程序与管理程序](https://magiskmanager.com/)([github](https://github.com/topjohnwu/Magisk/releases))
* 分开安装
```
adb install MagiskManager-v7.5.1.apk
adb push twrp-pixel-installer-sailfish-3.2.3-1.zip /data/local/tmp
adb reboot bootloader
fastboot boot twrp-3.2.3-1-sailfish.img
fastboot reboot
adb push Magisk-v20.3.zip /data/local/tmp 
adb reboot bootloader
fastboot boot twrp-3.2.3-1-sailfish.img
```











