---
description: 下载:https://github.com/2dust/v2rayN/releases
---

# 如何使用v2rayN

注意：新手请下载自带内核的版本。

文件说明：

#### windows x64

* v2rayN-With-Core.zip 包含所有Core文件，如您第一次请下载此包
* v2rayN.zip 不包含Core文件
* zz-v2rayN-With-Core-SelfContained.7z，包含所有Core文件；独立包，不需要下载安装\[Microsoft .NET 6.0 Desktop Runtime]\(有问题不推荐)

#### windows x86

* v2rayN-32.zip 不包含Core文件

#### windows arm64

* v2rayN-arm64.zip 不包含Core文件

\
提示：旧版似乎32位和64位通用，但核心依据系统位数运行。32位系统的小伙伴请先点击检查更新——\*\*\*\* Core以下载核心，或者按照下方的信息提示下载对应的文件。

有可能因为版本更新，界面有所不同，写这个教程时V2rayN最新版是6.23

首先将程序解压出来，在文件夹中找到v2rayN.exe打开就能启动程序了，如果嫌麻烦可以右键发送快捷方式到桌面。

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 233225.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 232907.png" alt=""><figcaption></figcaption></figure>

**一.功能说明**

Ⅰ.点击"服务器"可以添加节点

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 232616.png" alt=""><figcaption></figcaption></figure>

解释一下：

1.添加\[xxx]服务器：添加xxx协议的服务器(手动配置)

2.从剪贴板导入批量URL：检测剪贴板是否包含有效的订阅链接并添加

* VMESS服务器即v2Ray节点地址：`vmess://`
* VLESS服务器即Xray节点地址：`vless://`
* Shadowsock服务器节点地址：`ss://`
* Socks服务器节点地址：`socks5://`
* Trojan服务器节点地址：`trojan://`

注意一定要复制全。

3.扫描屏幕上的二维码：自动扫描屏幕上的二维码已添加节点

Ⅱ.点击"订阅分组"可以对所以订阅组进行管理和更新

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 232654.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 234235 (1).png" alt=""><figcaption></figcaption></figure>

下方信息栏出现如下字样即为更新订阅成功：

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 234600.png" alt=""><figcaption></figcaption></figure>

Ⅲ.点击"设置"进行各项参数设置

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 232707.png" alt=""><figcaption></figcaption></figure>

**二.使用**

选择服务器：服务器列表选择一个服务器右键点击"设为活动服务器"(或按回车)即可

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 232923.png" alt=""><figcaption></figcaption></figure>

任务栏找到如下图标并右键会打开简易配置界面

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 233031.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 233004.png" alt=""><figcaption><p>配置界面</p></figcaption></figure>

大体界面上和旧版本是一样的，但我们右键任务栏的时候会发现。。。HTTP代理没了。。。

新版本将HTTP代理改成了系统代理，这三个选项可以简单理解为

清除系统代理——不开启代理

自动配置系统代理——开启代理(默认全部能走代理的流量进\*ray，然后就跟据路由分流区别出国内外流量，国外流量全部走代理，需配合geoip和geosite)

不改变系统设置——不改变现有代理状态

pac模式——黑名单（如gfwlist.txt）模式(只有在黑名单上的域名才会走代理)

如上图配置可以实现精准代理，让该代理的走代理，国内的不走代理。

但上图的配置无法打开ChatGPT,要打开ChatGPT，请打开软件目录下的guiConfig/pac.txt中添加如下配置：

<figure><img src="../.gitbook/assets/屏幕截图 2023-08-06 221626.jpg" alt=""><figcaption></figcaption></figure>

若要突破有地区限制的网站请配置为如下模式：

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 233016.png" alt=""><figcaption></figcaption></figure>

提示：可以自己配置路由但新手掌握这两种模式就够了。

至此就可以翻墙上网了。

**三.订阅设置**

点击界面中的"+"号即可添加分组(订阅组)

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 232733.png" alt=""><figcaption></figcaption></figure>

1.别名：随便一个名称

2.可选地址：你的订阅地址

_提示：建议打开"启用更新"并设置"自动更新间隔"为"1"_

**四.分享**

节点分享：在列表中选择节点并右键点击"分享服务器"即可

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 232923 (1).png" alt=""><figcaption></figcaption></figure>

订阅分享：打开订阅分组——订阅分组设置再点击"分享"即可分享订阅

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 234235.png" alt=""><figcaption></figcaption></figure>

**四.问题解答**

1：为什么已按教程配置但无法打开Google等网站(Win10以上)？

解决：进入[ms-settings:network-proxy](ms-settings:network-proxy)并勾选"自动检测设置"

2：为什么在关闭其它代理软件后V2rayN失效了？

解决：点击界面的"重启服务"即可

提示：若要使用多个代理，建议使用[SwitchyOmega](https://github.com/FelisCatus/SwitchyOmega/releases)管理代理程序([教程](https://switchyomega.org/))

<figure><img src="../.gitbook/assets/屏幕截图 2023-06-28 233042.png" alt=""><figcaption></figcaption></figure>

3：Windows 8以上UWP/Metro应用无法联网：

点击设置——解除Win10UWP回环代理限制，并按如图操作：

<figure><img src="../.gitbook/assets/屏幕截图 2023-09-12 233331.png" alt=""><figcaption></figcaption></figure>

