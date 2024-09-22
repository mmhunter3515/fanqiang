# 如何配置 Shadowrocket 小火箭 vpn
Shadowrocket 等第三方工具允许您管理特定用例的代理服务器。幸运的是，Oxylabs 代理可以轻松与 Shadowrocket 应用程序集成。在本指南中，我们将逐步解释如何将我们的[住宅]、[移动]和[数据中心代理]与 Shadowrocket 集成。
如果您想在 YouTube 上查看集成过程，请点击下面的视频：

## **下载 Shadowrocket**

要[安装 Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118)，只需前往 App Store 并将应用程序下载到您的 iOS 设备。

## **使用代理设置 Shadowrocket**

**1.添加服务器。** 

要将我们的代理与 Shadowrocket 一起使用，首先打开 Shadowrocket 应用程序，然后单击**添加服务器**_。_

![](/_next/image?url=https%3A%2F%2Foxylabs.io%2Foxylabs-web%2FZpA9nh5LeNNTxDvm_OWQ4ZDE0YTMtMDE0NC00MDA0LThjZGEtYTg1MzExMDdlNzBh_shadowrocket-1-.png%3Fauto%3Dformat%2Ccompress&w=3840&q=75)

在以下窗口中，单击**类型**_。_

![](/_next/image?url=https%3A%2F%2Foxylabs.io%2Foxylabs-web%2FZpA9nx5LeNNTxDvn_YTVkYTU2MTctNjRkYi00M2Q1LTkwNjItMzFmN2FlYjUwNjM0_shadowrocket-2.png%3Fauto%3Dformat%2Ccompress&w=3840&q=75)

选择一种**类型**（继续阅读有关代理类型的详细信息）并返回上一屏幕。

![](/_next/image?url=https%3A%2F%2Foxylabs.io%2Foxylabs-web%2FZpA9oB5LeNNTxDvo_41557dbc-ca1c-4327-8ac9-53e15352f25a_shadowrocket-img4.png%3Fauto%3Dformat%2Ccompress&w=3840&q=75)

**2\. 输入代理和身份验证信息。** 

### 住宅和移动代理

**类型：**HTTP、HTTPS或SOCKS5

**地址：**pr.oxylabs.io

**港口：**7777

您还可以使用特定国家/地区的条目。例如，在**代理 IP下输入**us-pr.oxylabs.io并在**代理端口下输入**10000将获取美国出口节点。请参阅我们的[文档](https://developers.oxylabs.io/proxies/residential-proxies/country-specific-entry-nodes)以获取特定国家/地区入口节点的完整列表，或者您是否需要[粘性会话](https://developers.oxylabs.io/proxies/residential-proxies/session-control/sticky-proxy-entry-nodes)。[](https://developers.oxylabs.io/proxies/residential-proxies/country-specific-entry-nodes)[](https://developers.oxylabs.io/proxies/residential-proxies/session-control/sticky-proxy-entry-nodes)

### 数据中心代理

**类型：** HTTP、HTTPS或SOCKS5

**地址：** dc.oxylabs.io

**端口：** 8001

对于**按 IP 付费**订阅，端口是分配给给定列表中 IP 地址的序列号。因此，端口8001使用列表中的第一个 IP 地址。有关更多详细信息，请查看我们的[文档](https://developers.oxylabs.io/proxies/datacenter-proxies/proxy-list)。

对于**按流量付费**订阅，端口8001会选择一个随机 IP 地址，但在会话期间保持一致。您还可以在用户身份验证字符串中指定地理位置，例如美国：user-USERNAME-country-US:PASSWORD。查看我们的[文档](https://developers.oxylabs.io/proxies/datacenter-proxies/ip-control)了解更多详细信息。

### 企业专用数据中心代理

**类型：**HTTP或SOCKS5

**地址：**特定 IP 地址（例如1.2.3.4）

**端口：** 60000

对于企业专用数据中心代理，您必须从获取的列表中选择一个 IP 地址。请访问我们的[文档](https://developers.oxylabs.io/proxies/dedicated-datacenter-proxies/enterprise/proxy-lists)了解更多详细信息。

### 自助服务专用数据中心代理

**类型：**HTTP、HTTPS或SOCKS5

**地址：**ddc.oxylabs.io

**港口：**8001

对于自助服务专用数据中心代理，端口表示从获取的列表中 IP 地址的序列号。查看我们的[文档](https://developers.oxylabs.io/proxies/dedicated-datacenter-proxies/self-service/proxy-list)了解更多详细信息。

### ISP 代理

**类型：**HTTP、HTTPS或SOCKS5

**地址：**isp.oxylabs.io

**港口：**8001

**无论代理类型如何，都不要忘记在用户** 和**密码**下输入您的 Oxylabs 代理用户凭据。完成后，按后退箭头返回上一屏幕。 

**注意**：有关其他 Oxylabs 代理定制选项（例如特定国家/地区的入口点），请分别参阅[共享数据中心](https://developers.oxylabs.io/proxies/shared-datacenter-proxies/select-country)和[住宅代理](https://developers.oxylabs.io/proxies/residential-proxies/location-settings/country-specific-entry-nodes)文档。

![](/_next/image?url=https%3A%2F%2Foxylabs.io%2Foxylabs-web%2FZpA9oR5LeNNTxDvp_6e7ac4b3-8f02-419f-87c0-0fb19a9260e0_Shadowrocket-4.png%3Fauto%3Dformat%2Ccompress&w=3840&q=75)

**3.开启代理。**

填写代理详细信息后，您将能够打开代理。为此，请激活**“未连接”下的切换按钮**_。_

![](/_next/image?url=https%3A%2F%2Foxylabs.io%2Foxylabs-web%2FZpA9oh5LeNNTxDvq_NmMzYzU1ZDMtNTQ1Yy00MjY1LTlmNWMtYzVkZjdlOGRmYjQ5_shadowrocket-5.png%3Fauto%3Dformat%2Ccompress&w=3840&q=75)

如果这是您第一次使用 Shadowrocket，您将收到 iOS 提示，要求将 Shadowrocket 添加到您的 VPN 配置中，然后安装 VPN 配置文件。单击**添加**，然后 **好的**。您需要输入您的 iPhone 密码进行确认。

![](/_next/image?url=https%3A%2F%2Foxylabs.io%2Foxylabs-web%2FZpA9ox5LeNNTxDvr_21ceae6b-4bb7-47d7-a510-f7e422fcd9bc_shadowrocket-img3.png%3Fauto%3Dformat%2Ccompress&w=3840&q=75)

就是这样。应用程序顶部的切换按钮现在应该被激活了。

![](/_next/image?url=https%3A%2F%2Foxylabs.io%2Foxylabs-web%2FZpA9pB5LeNNTxDvs_YjU5MmVmOTQtMDMxOC00YWUyLTg4NWYtYjc2MDIzNTBkNDM3_shadowrocket-7.png%3Fauto%3Dformat%2Ccompress&w=3840&q=75)

**4\. 测试您的代理。**

[您可以通过访问ip.oxylabs.io](https://ip.oxylabs.io/)轻松测试代理是否正常工作。

## **快速设置教程**

为了您的方便，下面是使用代理设置的 Shadowrocket 的快速视觉演示：

![](/_next/image?url=https%3A%2F%2Foxylabs.io%2Foxylabs-web%2FZpA9ph5LeNNTxDvt_NzAxODc1YTMtM2Y4Mi00Yjc0LWJhNTYtNWIyYjg4OTYyMmE2_shadow-rocket.gif%3Fauto%3Dformat%2Ccompress&w=3840&q=75)

## **结论** 

Shadowrocket 与 Oxylabs 代理结合使用，可为您的 iOS 设备提供额外的安全性和隐私性。同样，请查看[Android 的 Shadowrocket 代理集成](https://oxylabs.io/resources/integrations/shadowrocket-android)。

Shadowrocket 代理与 Oxylabs 代理的集成快速而简单，因此您可以立即开始开展项目。如果您对集成 Oxylabs 代理有任何疑问，请随时联系我们。

_请注意，这是一个第三方工具，不归 Oxylabs 所有或控制。每个第三方提供商都对其自己的软件和服务负责。因此，Oxylabs 对这些服务不承担任何责任。在访问或使用第三方服务之前，请仔细查看第三方的政策和做法和/或进行尽职调查。_

## 常见问题

### Shadowrocket 是什么？

Shadowrocket 是一款规则驱动的实用应用程序，可让用户监控流量并从各个位置访问网站。此外，该应用程序还提供评估网站安全性的功能。它可供 Windows、Mac 和 Android 下载。

### Shadowrocket 安全吗？

Shadowrocket 允许用户在保持匿名的情况下访问互联网。Shadowrocket 应用程序使用多种加密方法来保护您的数据。

### 我可以将 SOCKS5 代理与 Shadowrocket 一起使用吗？

是的，可以将 SOCKS5 代理与 Shadowrocket 一起使用。为此，请确保您使用的是专用数据中心代理以及**类型**字段中的正确协议。
