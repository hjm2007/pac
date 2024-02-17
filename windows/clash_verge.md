---
description: 下载:https://github.com/clash-verge-rev/clash-verge-rev/releases
---

# 如何使用Clash Verge

如果无法启动，请安装[WebView2](https://go.microsoft.com/fwlink/p/?LinkId=2124703)

1.打开软件后，点击托盘图标后，点击"新建"已创建配置:

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

2.依据情况配置:

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

解释:

`①Remote` 和 `Local` 类型为 **主配置文件**，`Script` 和 `Merge` 类型为 **增强配置文件**，用于修改主配置文件的。

②[Remote 远程配置](https://clash-verge-rev.github.io/guide.html#remote-%E8%BF%9C%E7%A8%8B%E9%85%8D%E7%BD%AE):目前仅支持 clash 格式的配置链接，即响应体数据是符合 clash 配置格式的（utf8 编码）。如果响应头中存在 `Subscription-Userinfo` 字段，则其对应的流量信息会展示出来。远程配置可以点击右上角的更新按键自动更新。

③[Local 本地配置](https://clash-verge-rev.github.io/guide.html#local-%E6%9C%AC%E5%9C%B0%E9%85%8D%E7%BD%AE):新建本地配置之后，`右键 - 打开文件` 即可打开对应的本地配置文件（默认会用 VScode 打开，如果找不到执行程序则用默认编辑器打开）。在编写完本地配置之后`右键 - 使用` 即可刷新该配置。

4.配置完成后，点击代理并选择适合的选项

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

5.再点击"设置——系统代理"即可上网

提示:可在设置配置中文
