---
description: 下载:https://1.1.1.1或https://one.one.one.one
---

# 如何使用Cloudflare WARP

Notes:由于已经安装，所以部分图片来自网络。

条件(临时)：有一个很好的梯子

**1.下载并安装Cloudflare WARP**

<figure><img src="https://cdn.jsdelivr.net/gh/Misaka-blog/imgs@main/20230208121804.png" alt=""><figcaption></figcaption></figure>

#### 2.启动客户端并连接节点 <a href="#qi-dong-ke-hu-duan-bing-lian-jie-jie-dian" id="qi-dong-ke-hu-duan-bing-lian-jie-jie-dian"></a>

我们如果正常启动CloudFlare WARP时候，由于注册服务域名被GFW阻断，因此就有可能遇到无法注册的问题。

1. 第一次打开客户端之前，需要打开代理软件的真全局模式
2. 进入设置选项，如Device ID出现非0000的字符串时，即为注册成功

<figure><img src="https://cdn.jsdelivr.net/gh/Misaka-blog/imgs@main/20230208121824.png" alt=""><figcaption></figcaption></figure>

3. 断开并关闭代理软件，连接WARP。如出现Connected即为连接成功

<figure><img src="https://cdn.jsdelivr.net/gh/Misaka-blog/imgs@main/20230208121841.png" alt=""><figcaption></figcaption></figure>

_注意:如一直处在Connecting状态，则说明目前WARP服务已被GFW阻断_

**3.优选IP**

为什么优选IP：正常状态下WARP连接概率很小，需要我们对其IP进行优选\
1.下载工具:[https://github.com/hjm2007/download/blame/main/ip.zip](https://github.com/hjm2007/download/blame/main/ip.zip)

2.运行"1：生成优选IP端口结果文件.bat"(请关闭代理)

3.依据情况选择(建议默认)

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 170704.png" alt=""><figcaption></figcaption></figure>

4.在出现如下提示打开"result.csv"，复制第二行的IP(如图):

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 170923.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 171014.png" alt=""><figcaption></figcaption></figure>

5.管理员运行"2：将选好的ip复制到这里.bat",再将优选的IP复制到这里，若出现如下提示即可完成优选

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 171041.png" alt=""><figcaption></figcaption></figure>
