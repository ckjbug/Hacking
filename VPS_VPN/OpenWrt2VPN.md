## 使用基于OpenWrt的软路由实现科学上网
<div align="center">
    <img src="https://avatars0.githubusercontent.com/u/2528830?s=200&v=4">
    <br>
</div>
![](https://raw.githubusercontent.com/ckjbug/xiaokui/master/split.png)

#### OpenWrt是什么？

OpenWrt是一个嵌入式Linux发行版，可以安装在各种路由器上。OpenWrt有一个Web界面，它可能比您硬件的默认固件更稳定。

#### OpenWrt有什么功能？

- 使用SSH服务器进行SSH隧道：OpenWrt包含SSH服务器，因此您可以访问其终端。如果将SSH服务器暴露给Internet（确保使用基于密钥的身份验证而不是弱密码来保护它），则可以远程访问它并使用SSH隧道通过加密连接转发流量。这使您可以安全地从公共Wi-Fi访问网站，并访问只能在国外旅行时访问的网站。
- 设置VPN：SSH隧道 在很多方面与VPN类似，但您也可以在OpenWrt路由器上设置合适的VPN。
安装BitTorrent客户端：通过某种网络连接存储  或带有集成USB端口和连接USB存储设备的路由器，您可以将路由器本身用作BitTorrent客户端。
- 运行服务器软件：OpenWrt的软件存储库包含允许其用作Web服务器，IRC服务器，BitTorrent跟踪器等的软件包。您可能已经在使用路由器了，那么为什么不使用与服务器相同的路由器功能呢？对于初学者来说，路由器所需的功率远低于计算机。
- 执行流量整形和QoS：OpenWrt允许您对通过路由器的数据包执行流量整形和服务质量，优先处理某些类型的流量。您甚至可以优先处理流向特定计算机的流量，确定流向其他计算机的流量的优先级。
- 创建访客网络：OpenWrt的Wiki包含为访客设置特殊无线网络的说明，为了安全起见，该网络与主网络分开。您甚至可以限制访客网络的速度。
- 捕获和分析网络流量：您可以使用tcpdump将通过路由器传输的所有数据包记录到网络共享，并使用Wireshark等工具打开文件，以分析网络流量。

这不是一个完整的列表，不是一个长镜头 - 但它应该让你思考OpenWrt可能做什么。它是一个嵌入式Linux系统，提供各种各样的软件包，并且在很多方面它都像运行Linux的计算机一样灵活 - 尽管它的硬件受到更多约束。


#### 为什么使用OpenWrt制作软路由？

如果您对将路由器变为SSH服务器，VPN，流量整形系统或BitTorrent客户端的想法垂涎三尺 - 请考虑使用OpenWrt。


#### 怎么配置OpenWrt软路由实现科学上网？

---------


[OpenWrt开源项目](https://github.com/openwrt)
