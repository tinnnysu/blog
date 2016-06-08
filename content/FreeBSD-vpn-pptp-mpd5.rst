FreeBSD10.1 搭建PPTP服务器
================================

:date: 2015-01-15 10:40
:modified: 2015-01-15 10:40
:tags: FreeBSD,MPD5,PPTP
:category: 网络
:slug: freebsd-pptp 
:authors: htstudios
:summary: PPTP

最近频繁更换服务器，各种重装，各种配置，VPN服务是不可或缺的，每次配置都需要
Google，索性翻译过来，还可以深入学习一下。

原文地址：http://www.netroby.com/view.php?id=3598

安装要求
-----------------------

#. FreeBSD 10.1
#. 基于KVM的VPS或独立服务器
#. 能够使用ssh配置你的服务器
#. 能够使用FreeBSD Ports系统编译安装软件
#. 能够通过Google查找答案（还是Google好用些）

**注意**

**使用你的IP地址替换 27.12.32.17**

安装步骤
----------------------

#. 编译 `mpd5 <http://www.freshports.org/net/mpd5/>`_ 并选择使用 
   `ng_ipacct <http://www.freshports.org/net-mgmt/ng_ipacct/>`_ 。

   cd /usr/ports/net/mpd5
   make install clean

#. Test



