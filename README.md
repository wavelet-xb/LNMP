ShadowsocksR
===========

帮助您绕过防火墙的快速隧道代理.

服务端
------

### 安装

Debian / Ubuntu:

    apt-get install git
    git clone https://github.com/wavelet-xb/shadowsocksr.git

CentOS:

    yum install git
    git clone https://github.com/wavelet-xb/shadowsocksr.git

Windows:

    git clone https://github.com/wavelet-xb/shadowsocksr.git

### linux平台上的单用户使用

如果你把它克隆到 "~/shadowsocksr"  
移动到 "~/shadowsocksr", 然后运行:

    bash initcfg.sh

移动到 "~/shadowsocksr/shadowsocks", 然后运行:

    python server.py -p 443 -k password -m aes-128-cfb -O auth_aes128_md5 -o tls1.2_ticket_auth_compatible

通过检查所有选项 `-h`.

也可以改用配置文件（推荐）, 移动到 "~/shadowsocksr" 然后编辑文件 "user-config.json", 然后转到 "~/shadowsocksr/shadowsocks" 再来一次, 就跑:

    python server.py

在后台运行:

    ./logrun.sh

停止:

    ./stop.sh

监视日志:

    ./tail.sh


客服端
------

* [Windows] / [macOS]
* [Android] / [iOS]
* [OpenWRT]

在本地PC/手机上使用GUI客户端.查看客户的自述文件
更多信息.

文档
-------------

您可以在[Wiki]中找到所有文档.

许可证
-------

版权所有2015 clowwindy

根据Apache许可证2.0版（以下简称“许可证”）授权；您可以
除非符合许可证, 否则不要使用此文件.你可以获得
许可证副本

    http://www.apache.org/licenses/LICENSE-2.0

除非适用法律要求或书面同意, 否则软件
根据许可证分发的是按"原样"分发的, 而不是
明示或默示的任何形式的保证或条件.见
管理权限和限制的特定语言的许可证
在许可证下.
