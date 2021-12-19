
# 1. 前提

MerlinClash 至少运行在官改固件上，请您首先点开路由器管理界面 

查看固件版本，如果是官方版本，请您下载官改固件并刷机

[点我打开koolshare论坛下载官改固件](https://firmware.koolshare.cn/)

本教程依靠华硕GT-AC5300为例编写，其他路由器可参照本教程适当调整


# 2. 获取应用
注意：请根据您的路由器型号选择下载，建议关注Telegram频道以获取最新版本 

1. 将下载的文件重命名为 merlinclash.tar.gz  (全小写)

2. 然后回到路由器界面，进入软件中心 - 离线安装，选择文件并选择刚才的 merlinclash.tar.gz 文件

3. 点上传并安装，稍等片刻就安装好了

[网盘下载1](https://www.lanzoui.com/b07xyfrtg)
[Telegram频道下载](https://t.me/merlinclashcat/241)

![](https://pic.233.mx/images/2021/05/06/YcRWrTEfJ5OGHnI.png)
![](https://pic.233.mx/images/2021/05/06/VdB7QYqwTJI4vum.png)

# 3. 解除限制

注意：koolshare等可能提示插件非法无法安装，就需要操作这步，如果没提示直接跳过即可

1. 在软件中心安装 shellinabox（直接从未安装列表点击可直接安装）

2. 打开 shellinabox  并输入路由器登陆用户名和密码进行登陆

3. 复制以下代码  右击粘贴到shellinabox界面 然后按回车运行

sed -i 's/\tdetect_package/\t# detect_package/g' /koolshare/scripts/ks_tar_install.sh

![](https://pic.233.mx/images/2021/05/06/4zi8g3TtRKS5W9I.png)

# 4. 配置订阅

1. 到官网订阅中心选择复制订阅，然后回到路由器里打开刚安装好的插件 

2. 粘贴复制到的订阅到 SubConverter本地转换 中，然后点 开始转换 

3. 之后会自动进行配置，最后返回到界面，此时已完成启用。

![](https://pic.233.mx/images/2021/05/06/yaspmM3K2Tko1xP.png)

# 5. 开启代理

1. 如果没自动启用，就打开插件的 首页功能 ，配置文件选择刚才生成的这个文件

2. 然后划到最底下点 保存&amp;应用，然后打开 Merlin Clash开关

3. 稍等片刻就可以看到上面的插件运行状态一片绿色就是可以了

4. 如果要设置分流可以点下面两个按钮打开图形界面设置

![](https://pic.233.mx/images/2021/05/06/SpElh7nFOq3stGQ.png)
![](https://pic.233.mx/images/2021/05/06/kaq2RwZQ69yFhTX.png)