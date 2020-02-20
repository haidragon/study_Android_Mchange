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


## 编译源码







