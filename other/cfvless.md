---
description: 注意:此方法IP地址有跳动风险，请尽量不要登陆常用账号
---

# 使用CF Worker搭建vless节点

### 一.准备

1.Cloudflare账户

2.域名(可到eu.org注册且要绑定Cloudflare)

### 二.搭建

1.进入CF官网，点击"Workers 和 Pages——创建应用程序"

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

2.随便取个名字后点"部署"

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

3.点击编辑代码，在[这里](https://github.com/3Kmfi6HP/EDtunnel/blob/main/\_worker.js)获取。

提示:

( 1 )在`let userID = 'd342d11e-d424-4583-b36e-524ab1f0afa4';`处的"d342d11e-d424-4583-b36e-524ab1f0afa4"替换为自己生成的UUID，可以到[这里](https://1024tools.com/uuid)免费生成

( 2 )如下代码段为自定义伪装网址，可根据情况修改:

<pre><code>//伪装网站名单
const hostnames = ['www.fmprc.gov.cn', 'www.xuexi.cn', 'www.gov.cn', 'mail.gov.cn', 'www.mofcom.gov.cn', 'www.gfbzb.gov.cn', 'www.miit.gov.cn', 'www.12377.cn'];
<strong>//伪装网站域名(可换为url.hostname = ['www.example.com'];其中www.example.com是你用于伪装的网站域名)
</strong><strong>url.hostname = hostnames[Math.floor(Math.random() * hostnames.length)];
</strong>url.protocol = 'https:';
</code></pre>

3.点击"保存并部署"

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

4.回到概述,点击"触发器"可在"自定义域"处绑定你的域名

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

5.打开"https://<你绑定的域名>/<你的UUID>"即可查询节点信息

### 附.CF Pages搭建

使用CF Pages搭建，还需要一个Github账号并Fork项目[https://github.com/3Kmfi6HP/EDtunnel](https://github.com/3Kmfi6HP/EDtunnel)参考前面的方法即可。

**2024-4-5:**可以通过代理赛风VPN实现节点地区固定，仅需在赛风中设置上游代理为节点代理地址，再选择地区即可(地区有限)。详细教程请参考[这里](https://www.youtube.com/watch?v=y7dJvu1dbE0)
