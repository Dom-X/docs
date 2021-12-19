
# 1. 概述

Clash 是一个基于Go语言开发的跨平台代理程序。

Clash For Linux 是基于 Electron 和 Clash 开发的 Linux 代理程序，可以让用户通过 GUI 直观的对 Clash 进行配置。

# 2. 下载并安装 Clash for Linux

[网盘下载1](https://www.lanzoui.com/b07xybeid)

[网盘下载2](https://cowtransfer.com/s/17aae89db90543)

[github下载](https://github.com/Dreamacro/clash/releases/download/v1.2.0/clash-linux-amd64-v1.2.0.gz)

# 3. 配置

1. 创建你想要的存放文件的目录，解压gz包，我存放的路径是/root/clash，可以将解压文件重命名为clash便于阅读

`unzip /clash-linux-amd64-v0.18.0.gz`

2. 赋予文件执行权限

`chmod +x clash`

3. 启动文件

`./clash`

第一次启动会在用户目录下自动生成Config.yaml 和Country.mmdb两个文件。

生成的Config.yaml文件为空，需要后续填写自己的代理信息。

我这里生成的目录是/root/.config/clash，如果不一致的话可以使用find命令查找一下

4. 添加 Clash 配置订阅

到官网订阅中心选择复制订阅，然后在浏览器中访问【 订阅地址后面加&amp;flag=clash 】 ，然后右击浏览器页面，选择“另存为”保存页面

然后给保存的文件修改为Config.yaml （格式也要修改）

然后我们编辑下文件内容

首先把`port: 7890`这一行前面的全删掉

然后把`&lt;/body&gt;&lt;/html&gt;`这一行删掉

修改完成以后保存 替换掉刚才解压出的空的Config.yaml文件

5. 启动clash

配置完成后重新执行命令启动clash，以加载修改的配置文件

打开下面的网址访问管理页面

[http://clash.razord.top/#/proxies](http://clash.razord.top/#/proxies)

6. 设置虚拟机网络，配置代理

以 centos7.4 为例，打开系统设置，选择网络，点击网络代理，选择手动，按照yml配置文件中设置的端口进行配置，填写 HTTP 和 HTTPS 代理为 127.0.0.1:7890，填写 Socks 主机为 127.0.0.1:7891，即可启用系统代理

# 4. 设置分流

点击窗口左侧的 Proxies (代理)

默认情况下，Clash 使用 Rule (规则) 模式。不推荐选择 Global (全局) 与 Direct (直连) 模式。

Clash 支持通过策略组，对不同的网站使用不同的策略。合理使用分流可以提升您的使用体验。

Proxy 决策使用的线路，可在此处切换节点。

Domestic 决策所有中国大陆的网站，默认 DIRECT 为直连。

Global 决策在中国大陆无法访问的主流网站，默认 Proxy 为使用代理。

Others 决策不包含在 Global 规则内的冷门网站，默认 Proxy 为使用代理。

祝您使用愉快！
