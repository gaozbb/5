### 修改电脑名
永久修改
1.使用hostnamectl命令
hostnamectl set-hostname newname

2.修改配置文件/etc/hostname 保存退出
vi /etc/hostname
newname

临时修改主机名
hostname newname

查看主机名
hostname

查看本机名对应的ip地址
hostname -i


### 文件
1.建文件
touch file

2.进入目录
cd /etc

3.查看现有权限
ll

4.增加用户权限
chmod 777 file

5.切换用户
su 用户名

6.返回用户
exit

7.查看文件内容
cat file


### 挂载
1.卸载u盘设备
umount mnt/usb

2.挂载u盘至mnt下usb目录下
mount /dev/sdc1/mnt/usb

3.进入mnt
cd /mnt

4.查看分区使用情况
fdisk -l



### SSH秘匙
1.重置秘匙
ssh-keygen -t rsa -c "xxx@qq.com"

2.远程连接主机
ssh 主机名@ ip地址(ssh xxx@ 192.168.196.123)

3.拷贝远程文件
scp -r xx@192.168.192.123:/home/xx/xx/"filename" /home/tt/xx



### 用户、用户组
1.修改用户
usermod -l newuser olduser

2.修改用户组
groupmod -n newgroup oldgroup

3.把用户添加到某一个组里
useradd -a -g group user



### 磁盘目录
查看磁盘剩余空间
df -hl

返回目录大小
du -sh

该文件夹总文件数
du -sm

查看指定文件夹的大小
du -h

查看硬盘分区
fdisk -l

查看目录占用空间
du -hs



### 修改ip、网关
vim /etc/sysconfig/network