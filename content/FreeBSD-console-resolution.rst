FreeBSD Console Resolution
###############################

:date: 2015-01-17 9:23
:modified: 2015-01-17 9:23
:tags: FreeBSD,Console,分辨率
:category: FreeBSD
:slug: freebsd-console-resolution
:authors: htstudios
:summary: FreeBSD 控制台分辨率

随着服务器系统的更换，最近又换了笔记本的操作系统，索性将Windows去掉，只安装了
FreeBSD，用Windows的工作在公司做。

控制台
==========

FreeBSD中有两种控制台：sc和vt。可以通过查看相应的man pages来了解详情，FreeBSD
的man page做的真好，起码我感觉是这样的，Linux下我都没看过man pages，大多都看
不懂。今天的主题是vt，也叫Newcons。通过man pages可以知道，vt带来了很多好处，
支持UTF-8编码，与X Windows相结合，支持驱动更换
