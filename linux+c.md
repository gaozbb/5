tar打包，解包：
打包：tar -cvf xxx.tar 需要打包的文件
解包：tar -xvf xxx.tar 				不指定路径，默认当前路径解包
指定目录解包：tar -xvf xxx.tar -C	指定路径目录解包

查看目录大小：
du ./目录 -h

gzip压缩tar包
压缩：gzip xxx.tar			自动当前目录生成xxx.tar.gz
gzip -r xxx.tar xxx.tar.gz
解压：gzip -d xxx.tar

压缩打包：tar -czvf xxx.tar.gz	所需文件
解压解包：tar -xzvf xxx.tar.gz

压缩打包：tar -cjvf xxx.tar.bz2	所需文件
解压解包：tar -xjvf xxx.tar.bz2 -C	指定路径

压缩：zip -r test *	
解压：unzip -d 当前路径 解压文件


查看用户组信息：cat /etc/group
查看用户信息：cat /etc/passwd

修改文件权限：chmod u/g/o +/-/= r/w/x 文件名
修改文件所有者：chown 所有者 文件名
修改文件所属组：sudo chgrp 所属组 文件名

查看进程信息：ps -aux
杀死进程：kill 进程号
强力杀死：kill -9 进程号
查看动态进程：top

查看文件大小：ls -h
查看文件夹大小：du -h
查看磁盘大小：df -h

安装rpm包：rpm -ivh xxxxxxxxxxxx.rpm