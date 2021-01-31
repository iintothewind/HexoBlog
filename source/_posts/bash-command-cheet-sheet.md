---
title: bash command cheet sheet
date: 2020-05-03 11:53:32
tags: [linux,bash]
---

My WizNote service has been expired.
I did not pay to renew the service.
It is good and convenient though.
So I decided to move all my previous learning notes to here.
Most of them are not oringinally created by me.
I would try to include the source.
Please remind me to delete them if you are the author and you feel it is a violation of your IP.

```bash

# last parameter
$_

# word replace
^before^after

# check alias
type -a ll

alias sudo='sudo '
# greps
alias grep='grep --color'
alias egrep='egrep --color'
alias fgrep='fgrep --color'

# utils
alias sudo="sudo "
alias ll="ls -lthF"
alias la="ls -lthFA"
alias md="mkdir "
alias rm="rm -i"
alias mdate="date \"+%Y-%m-%d %H:%M:%S\""

# fedora
alias vim="gvim -v"
alias xcp="xclip -selection clipboard"
alias xcv="xclip -o"
alias rmrtlan="sudo route del default enp0s31f6"
alias scrnoff="xset dpms force off "
alias printpath="echo $PATH | tr : \\\\n"
alias lstcp="lsof -i -n -P | grep TCP"

# list top 5 files/ folders

du -h | sort -rh | head -n 5
# list only directories
ls -l | grep ^d

# tree list
find . -type d |sed 's:[^-][^/]*/:--:g; s:^-: |:'


find / -name file1  # 从 '/' 开始进入根文件系统搜索文件和目录
find / -user user1  # 搜索属于用户 'user1' 的文件和目录
find /home/user1 -name \*.bin    # 在目录 '/ home/user1' 中搜索带有'.bin' 结尾的文件
find /usr/bin -type f -atime +100   # 搜索在过去100天内未被使用过的执行文件
find /usr/bin -type f -mtime -10   #    搜索在10天内被创建或者修改过的文件
find / -name *.rpm -exec chmod 755 '{}' \;  # 搜索以 '.rpm' 结尾的文件并定义其权限
find / -xdev -name \*.rpm   # 搜索以 '.rpm' 结尾的文件，忽略光驱、捷盘等可移动设备
find ./code -name "*.c" |xargs grep -in "hello" # 在~/code目录搜索并显示文件名后缀为.c并且包含字符串hello的文件和行数
find . -type f -exec chmod 644 {} \;  #文件加644
find . -type d -exec chmod 755 {} \; ＃目录加755
find ./ -type f | xargs sudo chmod 644

# display thread

ps -efL
# display top 5 processes which has taken most memory and cpu resources
ps -ef --sort -pmem,+pcpu | head -n 6
# change output format
ps -eo pic,user,args
# monitor threads of process with name contains java
pidstat -C java -t

sudo localectl set-locale.utf8

wget -e use_proxy=on --no-check-certificate https://nodejs.org/dist/v5.1.0/node-v5.1.0-x64.msi
wget -t0 -c --no-check-certificate http://mirror.bit.edu.cn/apache/kafka/0.10.0.0/kafka_2.11-0.10.0.0.tgz -O ~/Downloads/kafka.tgz

# yum install and yum local install can both be replaced with:
sudo dnf install <anypackage>

# list services

systemctl list-unit-files | grep smb
# config service to be auto-start
systemctl enable smb.service
# start service
systemctl start service
# stop servie
systemctl stop service
# disable service
systemctl disable service

# copy .ttf font file to .fonts
$ fc-cache -vf

synclient TouchpadOff=1

# download a file, rename as amm, grant x permission, and run it.
$ curl -L -o amm https://git.io/vro0u && chmod +x amm && ./amm

$ watch --interval 1 date
# watch file size
$ watch -n60 du -h /var/log/messages

cut -d\    -f 1 ~/.bash_history | sort | uniq -c | sort -rn | head -n 10 | sed 's/.*/    &/g'
sudo -u apache find . -not -readable

# open connections
lsof -i | grep -E "(LISTEN|ESTABLISHED)"
# Displaying a Active Network Connections
lsof -i|grep -E "(LISTEN|ESTABLISHED)" |awk '{print $1, $8, $9}'
alias lsac="lsof -i | grep -E '(LISTEN|ESTABLISHED)'"

echo "Hello, world" | xclip
echo "Hello, world" | xclip -selection clipboard
xclip -sel clip < file
cat README.TXT | xsel
cat README.TXT | xsel -b # 如有问题可以试试-b选项
# 将readme.txt的文本放入剪贴板
xsel < README.TXT
# 清空剪贴板
xsel -c

sudo mkntfs -f -L udisk /dev/sdb1 -F

sudo dnf install fuse-exfat exfat-utils

docker images | tail -n +5 | head -n -1 | awk '{print $3}' | xargs docker rmi
```
