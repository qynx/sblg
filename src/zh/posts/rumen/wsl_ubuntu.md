---
icon: edit
date: 2022-11-08
category:
  - 入门
tag:
  - wsl
---

# wsl 配置

<!-- more -->

## 虚拟机安装

> wsl --list -o 可以查看在线版本

选择要安装的在线版本的name 如 (Ubuntu-18.04)

> wsl --install -d Ubuntu-18.04

如果安装速度过慢 可以直接在[官网](https://learn.microsoft.com/en-us/windows/wsl/install-manual)
下载对应版本


## ubuntu 软件下载镜像源


[清华镜像下载地址](https://mirrors.tuna.tsinghua.edu.cn/help/ubuntu/)

```
sudo vim /etc/apt/sources.list 替换文件中的内容
```

## pip 镜像配置

```bash
mkdir ~/.pip
vim ~/.pip/pip.conf
```

```
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
[install]
trusted-host = https://pypi.tuna.tsinghua.edu.cn
```