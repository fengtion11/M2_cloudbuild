https://github.com/openwrt-fork/zn-m2-openwrt-build/tree/zn-m2


<div align="center">
  <h1 align="center">
     IPQ60xx & MT798x 设备的 OpenWrt 固件发布页面
  </h1>
<a href="/LICENSE">
    <img src="https://img.shields.io/github/license/sdf8057/cloudbuild?style=flat&a=1" alt="">
  </a>
  <a href="https://github.com/sdf8057/cloudbuild/pulls">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat" alt="">
  </a><a href="https://github.com/sdf8057/cloudbuild/issues/new">
    <img src="https://img.shields.io/badge/Issues-welcome-brightgreen.svg?style=flat">
  </a><a href="https://github.com/sdf8057/cloudbuild/releases">
    <img src="https://img.shields.io/github/release/sdf8057/cloudbuild.svg?style=flat">
  </a><a href="hhttps://github.com/sdf8057/cloudbuild/releases">
    <img src="https://img.shields.io/github/downloads/sdf8057/cloudbuild/total?style=flat&?">
  </a>
</div>
<br>

## ipq6000固件特性：  
0.默认后台地址192.168.6.1；默认后台密码password。  
1.添加cpu温度、频率以及npu占用率显示。  
2.修复nat环回功能失效bug。  
3.cpu超频至1.6ghz，跑分2w+。  
4.为360/和目等设备添加原厂无线校准文件。  
5.支持在线安装软件，手动安装请确保插件使用lua语言编写。  
6.释放保留内存，可用内存增加50m。  
7.此页面发布的ipq6000固件不集成无线功能。  

## 集成插件列表
luci-app-ssr-plus  
luci-app-openclash  
luci-app-ddns  
luci-app-msd_lite  
luci-app-wol  
luci-app-upnp  
luci-app-uhttpd  
luci-app-cpufreq  
luci-app-ipsec-vpnd  
luci-app-openvpn-server  
luci-app-zerotier  

## 固件预览
感谢sdf8057、lean、kiddin大神！



本固件是从Github fork sdf8057/cloudbuild，KK2018gh/M2_cloudbuild，原版也是sdf8057的，修改config，将需要的app添加上，2月2日23年11月12日编译出来的版本，目前稳定运行。

本人Github地址：https://github.com/ws245909346/M2_cloudbuild（无releases，只供大家查看config、yml和diy文件）



适用于未修改运存（256MB）、不使用Wifi的和目AX18、ZN-M2。

在本人看来，只让路由器干路由器该干的活，这样路由器才能稳定，开机就不用管了，少到界面上操作，所以集成的App较少。



固件特点：

01.概览有NSS状态显示

02.CpuMark : 20709.293295分

03.Cpu最大频率可调：864-1608

04.含NSS加速

05.含端口回环

06.开机可用内存约140MB

07.支持ipv6



包含Applications：

01.luci-app-accesscontrol      时间控制

02.luci-app-arpbind                ARP绑定

03.luci-app-autoreboot           自动重启

04.luci-app-cpufreq                CPU最大频率设置

05.luci-app-ddns-go   luci-app-lucky            Lucky

06.luci-app-eqos                     IP限速

07.luci-app-fileassistant         Web端文件管理

08.luci-app-firewall                 防火墙

09.luci-app-ramfree                清除内存

10.luci-app-smartdns             优选DNS

11.luci-app-ttyd                       Web端终端

12.luci-app-turboacc              网络加速

13.luci-app-upnp                    自动端口转发

14.luci-app-wol                       网络唤醒

 15.k.m.s

包含Themes：

01.luci-theme-argonv3           Argon（防止与原版Argon冲突，sdf8057大神改的名）

02.luci-theme-bootstrap        系统自带主题（其他主题崩溃时使用）



分享源码（Github上查看）、config、固件包（包含Uboot版、Web端升级版，推荐使用Uboot安装固件，防止出现其他问题）和sha256比对，目的只有一个，请大家放心固件安全问题，源码我也不懂，反正用到的都是Github上的应用，本人也只会增加和删除固件功能。
