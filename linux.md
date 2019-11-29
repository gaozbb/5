### 系统信息

```markdown
arch									   显示机器的处理器架构
uname -m						   显示机器的处理器架构
uname -r							 显示正在使用的内核版本
dmidecode -q				   显示硬件系统部件
cat /proc/cpuinfo			 显示CPUinfo信息
cat /proc/version			 显示内核的版本
lsusb -tv							   显示USB设备
date									  显示系统日期
cal											查看日历
```

### 关机

```
shutdown -h now				关机
init 0										 关机
telinit 0								   关机
shutdown -c						   取消定时关机
shutdown -r now				  重启
reboot									  重启
```

### 文件和目录

```
cd /home									进入/home目录
cd ..												返回上一级目录
cd ../..										   返回上两级
cd ~user									  进入个人目录
cd -												返回上次所在目录
pwd												 显示工作路径
ls													  查看目录中的文件
ls -F												查看目录中的文件
ls -l												 显示文件和目录的详细资料
ls -a												显示隐藏文件
ls *[0~9]*									  显示包含数字的文件名和目录
tree											   显示文件和目录由根目录开始的树形结构
mkdir dir									 创建一个dir目录
mkdir -p /tmp/dir					创建一个目录树
rm -f file										删除一个叫file文件
rmdir dir									  删除一个dir目录
rm -rf dir									   最nb的删除（慎用）
mv dir new_dir						  重命名/移动文件
cp file1 file2								 赋值文件
cp dir/* .										复制一个目录中所有文件到当前目录
cp -a /tmp/dir .						复制一个目录到当前目录

ln -s file lnk												创建软连接
ln file lnk													  创建硬链接
touch -t YYMMDDhhmm file			 修改文件时间								
```

### 文件搜索
```
find / -name file							进入根文件系统搜索文件和目录
find / -user user1							搜索属于用户'user1'的文件和目录
find /usr/bin -type f -atime +100		搜索过去100天未被执行的文件
find /usr/bin -type f -mtime -10			搜索10天内被创建或者修改过的文件
```