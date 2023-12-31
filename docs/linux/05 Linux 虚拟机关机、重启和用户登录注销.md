---
title: Linux Vi和Vim编辑器
---
# Linux 虚拟机关机、重启和用户登录注销

## 关机&重启命令

### 基本介绍

+ <font color=#DC4040 size=4 face="黑体">shutdown   -h   now           立该进行关机</font>
+ <font color=#DC4040 size=4 face="黑体">shutdown    -h 1 "hello,1分钟后会关机了"</font>
+ <font color=#DC4040 size=4 face="黑体">shutdown   -r    now           现在重新启动计算机</font>
+ <font color=#DC4040 size=4 face="黑体">halt                                        关机，作用和上面一样.</font>
+ <font color=#DC4040 size=4 face="黑体">reboot                                   现在重新启动计算机</font>
+ <font color=#DC4040 size=4 face="黑体">sync                                       把内存的数据同步到磁盘.</font>

### 注意事项

+ 不管是重启系统还是关闭系统，首先要运行 sync命令，把内存中的数据写到磁盘中
+ 目前的 shutdown/reboot/halt等命令均已经在关机前进行了sync ，小心驶得万年船。

## 用户登录和注销

### 基本介绍

1. 登录时尽量少用root帐号登录，因为它是系统管理员，最大的权限，避免操作失误。可以利用普通用户登录，登录后再用”su-用户名’命令来切换成系统管理员身份.
2. 在提示符下输入logout即可注销用户.

### 使用细节

logout注销指令在图形运行级别无效，在运行级别3下有效.

