---
abbrlink: ltcq
categories: []
date: ''
image: https://tncache1-f1.v3mh.com/image/2025-09-24/6rI0cxTR32.jpg,https://tncache1-f1.v3mh.com/image/2025-09-24/tENKynWH49.jpg
tags: []
title: 雷霆传奇docker架设
updated: '2025-09-24T17:03:14.637+08:00'
---
本教程使用Centos 7.9演示搭建过程,建议使用Ubuntu 20.04、 Centos7.9和Debian10作为宿主机系统搭建。

测试使用2H4G服务器。

（一）安装docker和docker compose
1.更新系统 (系统更新不是必须，如果没法顺利安装docker和compose，可以尝试更新系统。)
Ubuntu20.04/Debian10
apt-get update && apt-get upgrade -y
Centos7
yum update -y

2.安装docker和docker compose
bash <(curl -sSL [https://linuxmirrors.cn/docker.sh](https://linuxmirrors.cn/docker.sh))
输入命令后按照引导进行安装。

（二）搭建服务端
1.把xjqx文件夹文件夹上传到服务器root目录，在线拉取镜像并创建容器
cd xjqx
docker compose up -d

2.登陆容器设置服务端并启动游戏
地址：ip:522   账号：root 密码：123456

配置服务端
cd /root && chmod 777 config && ./config    #根据引导完成脚本

启动和关闭游戏
cd /root && ./start.sh    #启动游戏
cd /root && ./stop.sh    #关闭游戏

3.游戏地址：http://你的外网ip:81

4.营运后台地址：http://你的外网ip:81/admin
账号：admin
密码：123456

5.GM后台
http://你的外网ip:81/gm
账号：admin
密码：123456

百度网盘链接：[https://pan.baidu.com/s/1OzzbjSfPEQir42jB0IPuJw?pwd=8brc](https://pan.baidu.com/s/1OzzbjSfPEQir42jB0IPuJw?pwd=8brc) 提取码: 8brc
视频教程链接：[https://www.bilibili.com/video/BV1xdpXzNEAJ/](https://www.bilibili.com/video/BV1xdpXzNEAJ/)

\*\*\*本教程只限于技术研究使用，请勿用于商业用途。\*\*\*

\*\*\*本教程资源全部来自互联网，仅供研究学习使用，下载后请于24小时内删除，或购买正版。\*\*\*
