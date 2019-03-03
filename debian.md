---
layout: base
---

# 通过网络最小化安装Debian后要做的事


1. 切换至root
```
$:su
```
2. 更新sources.list
```
先安装apt-transport-https
#:apt-get install apt-transport-https
前往 https://mirrors.ustc.edu.cn/repogen/ 选择合适版本的sources.list，下载并替换/etc/apt/sources.list，然后
#:apt-get update
#:apt-get upgrade
```
3. 安装vi/vim
```
#:apt-get install vim
```
4. 通过update-alternatives设定默认editor
```
#:update-alternatives --config editor
```
5. 通过visudo将用户加入sudo列表
```
#:visudo
```
6. 安装gcc
```
#:apt-get install gcc gdb
```
7. 安装make/cmake
```
#:apt-get install make cmake
```
8. 安装libtool
```
#:apt-get install libtool
```
9. 安装vm-tool
```
option
```
10. 添加ip信息/安装net-tools
```
#:ip address add $IP/24 dev $IF
```
11. 安装32位库/lib32ncurses5
```
#:apt-get install lib32ncurses5
```
12. 安装ctags
```
#:apt-get install ctags
```
13. 安装sudo
```
#:apt-get install sudo
```
14. 安装tftp
```
#:apt-get install tftp
```
15. 安装git
```
#:apt-get install git
```
16. 安装perl
```
#:apt-get install perl
```
17. 安装tree
```
#:apt-get install tree
```
18. 修改默认shell/dpkg-reconfigure dash
```
#:dpkg-reconfigure dash
```
19. 安装autoconf automake
```
#:apt-get install autoconf automake
```
20. 安装linux-headers-amd64
```
#:apt-get install linux-headers-amd64
```
21. 安装linux-source
```
#:apt-get install linux-source
```
22. 安装libncurses5-dev
```
#:apt-get install libncurses5-dev
```
23. 安装adb
```
#:wget https://dl.google.com/android/repository/platform-tools-latest-linux.zip
```
24. 配置vimrc
```
syntax on
filetype on
set title
set nu
set ai
set ts=4
set noexpandtab
set hlsearch
set ruler
```
25. 配置bashrc
```
option
```
26. 配置python默认版本
```
#:ln -s /usr/bin/python3 /usr/bin/python -f
```
27. 生成ssh key
```
$:ssh-keygen -t rsa -b 4096 -C "your@email.com"
$:ssh-copy-id your@domain.com
```