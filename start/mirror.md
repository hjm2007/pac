---
description: 针对部分设备无法访问
---

# 镜像站搭建指南

说明：因为国产浏览器和微信可能已屏蔽本项目的网址，所以推广时不太方便，所以如果制作一个本项目的镜像，得到一个新的网址，并定时同步，则更方便推广。

### 一.GitHub镜像

1、注册一个github.com账号，并登录；

2、打开 [https://github.com/hjm2007/pac](https://github.com/hjm2007/pac)

3、点右上角的Fork链接，fork完成后就得到了一个你自己的git翻墙教程的镜像网址。

但是fork的镜像不会自动跟随源项目而更新，怎么办呢？有2种办法:

方法1、每天手工更新，具体方法是删掉fork的项目，重新fork一下，就是最新的了。

具体是在Fork后的项目页面的顶部偏右的位置，有个Setting链接，点击Setting链接后，滚动到页面底部，点“Delete this repository”按钮，删除后重新Fork即可。

方法2、定时自动同步

你需要一台 **墙外（因为安全的原因,必须墙外）** 的Windows电脑或者Linux VPS,以Linux(Debian 10) VPS为例，首先，用ssh客户端登录linux，然后执行下列命令安装git工具：

```
apt update  
apt install git  
```

如果是windows电脑，请安装 [Git for Windows](https://git-scm.com/download/win)

然后，使用 SSH 连接到你的 GitHub账号(利用 SSH 密钥可以连接 GitHub，而无需在每次访问时提供用户名或密码，方便定时更新git翻墙教程镜像)\
参考:\
[https://docs.github.com/cn/github/authenticating-to-github/connecting-to-github-with-ssh](https://docs.github.com/cn/github/authenticating-to-github/connecting-to-github-with-ssh)

然后 Linux 则依次执行下列命令（一行一行依次拷贝执行,注意将your-github-username换作你自己的github用户名）：

```
cd /root  
git config --global core.autocrlf input  
git clone git@github.com:your-github-username/pac.git  
cd bnews  
chmod +x syncnews.sh  
git remote add upstream https://github.com/hjm2007/pac
```

然后将脚本 `/root/bnews/syncnews.sh` 加到你的linux crontab 里面定时执行即可。

Windows 则先打开Git CMD命令行，依次执行下列命令：

```
git config --global core.autocrlf true  
git clone git@github.com:your-github-username/pac.git  
cd bnews  
git remote add upstream https://github.com/hjm2007/pac  
```

这时，在当前这个 bnews 目录下会有一个 syncnews.bat 命令脚本，把这个命令脚本加入到windows的任务计划程序定时执行即可。

### 二.CF反代镜像

你可以参考[https://bili33.top/posts/CloudFlare-Workers/](https://bili33.top/posts/CloudFlare-Workers/)搭建CF Worker(CF Page)反代站，反代域名填写"winver-dev.gitbook.io"即可。

### 三.GitBook同步

1.注册一个Gitbook在线版并安装Github插件，同时注册一个github.com账号

2.打开前面的项目地址并Fork

3.参考[这里](https://zhuanlan.zhihu.com/p/343212233)进行同步，成功后即有一个镜像网站

### 四.GitBook CLI

可参考网上教程，需要对每个md文件进行更改
