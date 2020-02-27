# 第一课 Pixel刷谷歌官网rom包
* 第一步安装android studio(sdk)

```
安装完sdk后可能没有添加环境变量要自己手动添加(这里就不写了）
/Users/haidragon/Library/Android/sdk
进入platform-tools目录就会看到adb命令
export PATH=$PATH:/Users/haidragon/Library/Android/sdk/platform-tools

adb devices
adb reboot bootloader
export ANDROID_PRODUCT_OUT=./
echo $ANDROID_PRODUCT_OUT
./flash-all.sh
```
* 第二步去google官网下载对应的镜像文件，这里用的是[ Pixel](https://developers.google.cn/android/images#sailfish)随便下载个

* 第三步进入刚刚下载的目录下在刷入之前做一些必要的备份

```
直接运行flash-all.sh(注意官方镜像pixel系要全部刷入才能使用)
```









