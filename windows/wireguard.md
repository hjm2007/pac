---
description: 虽然使用WARP可以实现翻墙，但WARP注册服务域名被GFW阻断，因此困难巨大。所以，我们要将WARP配置文件转为WireGuard实现更自由科学上网。
---

# 如何使用WireGuard配合WARP进行科学上网

条件:务必打开WARP代理模式否则无法识别

1.下载并安装WireGuard:[https://www.wireguard.com/install/](https://www.wireguard.com/install/)

2.打开[https://replit.com/@ygkkkk/WARP-Wireguard-Register](https://replit.com/@ygkkkk/WARP-Wireguard-Register),点击"Run"

3.选"2"并回车

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 172325.png" alt=""><figcaption></figcaption></figure>

4.依据情况选择(这里为团队账户为例)

团队账户申请:[zero.md](../other/zero.md "mention")

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 172505.png" alt=""><figcaption></figcaption></figure>

5.依据提示获取Token并复制:

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 172621.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 172955.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 173115.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 173139.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 173225.png" alt=""><figcaption><p>被遮挡部分即为Token</p></figcaption></figure>

6.获取信息如下

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 173638.png" alt=""><figcaption></figcaption></figure>

7.复制上述配置信息，打开WireGuard，点击"新建新隧道"

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 173844.png" alt=""><figcaption></figcaption></figure>

8.粘贴配置文件至此

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 173919.png" alt=""><figcaption></figcaption></figure>

9.点击连接，出现如图即为连接成功

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-24 174207.png" alt=""><figcaption></figcaption></figure>

#### 2024年更新:自动分流

1.管理员cmd运行如下命令:

```
reg add HKLM\Software\WireGuard /v DangerousScriptExecution /t REG_DWORD /d 1 /f
```

2.进入[这里](https://github.com/lmc999/auto-add-routes/blob/master/zip/wireguard.zip)下载"wireguard.zip"并将里面的内容解压到WireGuard的安装目录

<figure><img src="../.gitbook/assets/捕获.PNG" alt=""><figcaption></figcaption></figure>

3.修改WireGuard节点配置文件。在MTU下方加入以下内容。取消勾选拦截未经隧道的流量前面的复选框。重新连接，之后就可以正常分流了。

```
PreUp = "C:\Program Files\WireGuard\routes-up.bat"
PostUp = "C:\Program Files\WireGuard\dns-up.bat"
PreDown = "C:\Program Files\WireGuard\routes-down.bat"
PostDown = "C:\Program Files\WireGuard\dns-down.bat"
```
