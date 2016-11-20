---
layout: post
title: 使用logrotate切割nginx日志文件
date: 2016-11-17 21:11:00 +800
categories: logrotate openresty nginx
---
## 在openresty(nginx)使用Logrotate切割日志
大体上有三种方法切割nginx日志。

第一种是写个定时任务，每天零点把旧的日志重命名，并对nginx进程发送USR1信号使其重新打开日志并写入。

第二种是能过管道的方式把新产生的日志写到另外一个日志文件里。

第三种是能过logrotate来切割日志，logrotate是系统自带的服务，可以切割任何日志，不仅仅是nginx，这里推荐使用它。

logrotate的配置文件是/etc/logrotate.conf，通常不需要对它进行修改。日志文件的轮循设置在独立的配置文件中，它（们）放在/etc/logrotate.d/目录下。
