---
description: 普通状态下WARP流量有限，无法满足我们的日常需求。这个教程将教你如何注册Cloudflare的团队账户实现无限流量
---

# 如何免信用卡申请Cloudflare Zero Trust实现无限流量

**由于本人已注册团队账户，所以本文为转载，有时间我会重新注册一个CF账号进行演示**

**原文地址：**[https://github.com/getsomecat/GetSomeCats/blob/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.md](https://github.com/getsomecat/GetSomeCats/blob/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.md)

条件(临时)：有一个很好的梯子，一个Cloudflare账户（自行百度）

1.登陆Cloudflare帐号，如果是新帐号，会有如下的一些提示：

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_12.17.52.png" alt=""><figcaption></figcaption></figure>

4.选择ZeroTrust，并且进入一些设置

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_12.19.10.png" alt=""><figcaption></figcaption></figure>

5.进入后要给你的组织取个名字，自己取一个好记住的就行，重复了会有提醒

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_12.19.48.png" alt=""><figcaption></figcaption></figure>

6.接下来是选择Plan

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_12.20.21.png" alt=""><figcaption></figcaption></figure>

7.跳过添加付款方式步骤

在上面选择好Plan后，到了添加付款方式页面，将地址栏：[https://one.dash.cloudflare.com](https://one.dash/cloudflare.com) 后面的全部删掉然后回车

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.02.36.png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.03.51.png" alt=""><figcaption></figcaption></figure>

8.跳转到了首页

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.04.31.png" alt=""><figcaption></figcaption></figure>

9.这时候点一下左侧的My Team，会发现里面没有东西

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_12.38.16-0168618.png" alt=""><figcaption></figcaption></figure>

10.点一下浏览器的后退接着按前进，My Team页面就会出现链接设备的选项了

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.07.28.png" alt=""><figcaption></figcaption></figure>

11.按照流程走完

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.07.59.png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.08.40.png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.09.22.png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.10.33.png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.11.13.png" alt=""><figcaption></figcaption></figure>

<figure><img src="https://github.com/getsomecat/GetSomeCats/raw/Surge/%E6%B3%A8%E5%86%8CCloudflare%E5%B9%B6%E5%8A%A0%E5%85%A5ZeroTrust%E6%95%99%E7%A8%8B.assets/iShot_2023-03-30_17.11.58.png" alt=""><figcaption></figcaption></figure>

这一套流程走完就可以关掉页面了，接下来就是去Cloudflare WARP设置了

11.WARP设置Teams

1. 打开客户端之前，需要打开代理软件的真全局模式
2. 打开WARP客户端
3. 按照下图操作

<figure><img src="https://cdn.jsdelivr.net/gh/Misaka-blog/imgs@main/20230208121927.png" alt=""><figcaption></figcaption></figure>

**近期在设备登录Zero Trust时会出现设备限制，解除请参考：blog.wudarensheng.top/p/2025**
