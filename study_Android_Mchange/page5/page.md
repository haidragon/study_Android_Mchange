# android 10版本源码编译与Pixel刷机

## 先下载android 10 源码

* 下载 repo工具

sudo apt-get install git

接下来创建bin，（可以加入到PATH中）

~: mkdir bin

下载 repo 设置权限

curl https://mirrors.tuna.tsinghua.edu.cn/git/git-repo > ~/bin/repo

设置从镜像中下载（tuna的镜像源）

export REPO_URL='https://mirrors.tuna.tsinghua.edu.cn/git/git-repo/'

设置身份，添加自己的邮箱和姓名:

git config --global user.email "piratemorgen@gmail.com" 

git config --global user.name "piratemorgen"

初始化

~/bin/repo init -u https://aosp.tuna.tsinghua.edu.cn/platform/manifest

指定版本

~/bin/repo init -u https://aosp.tuna.tsinghua.edu.cn/platform/manifest -b android-10.0.0_r29

同步

~/bin/repo sync -j10

![images](./1.png)
## 编译源码

[7za](https://blog.csdn.net/qq_27608983/article/details/92462659) a -v4g android-10.0.0_r29.7z ~/ 

7za x  android-10.0.0_r29.7z  -r -o./(-o后是没有空格的，直接接目录。这一点需要注意)

* 安装依赖项

```
sudo apt-get install -y libx11-dev:i386 libreadline6-dev:i386 libgl1-mesa-dev g++-multilib
sudo apt-get install -y git flex bison gperf build-essential libncurses5 
sudo apt-get install -y tofrodos python-markdown libxml2-utils xsltproc zlib1g-dev:i386
sudo apt-get install -y dpkg-dev libsdl1.2-dev libesd0-dev
sudo apt-get install -y git-core gnupg flex bison gperf build-essential
sudo apt-get install -y zip curl zlib1g-dev gcc-multilib g++-multilib
sudo apt-get install -y libc6-dev-i386
sudo apt-get install -y lib32ncurses5-dev x11proto-core-dev libx11-dev
sudo apt-get install -y libgl1-mesa-dev libxml2-utils xsltproc unzip m4
sudo apt-get install -y lib32z-dev ccache
sudo apt-get install -y libssl-dev

```











