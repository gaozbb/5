## 系统管理

### 防火墙(firewalld)

安装
~~~
sudo apt install firewalld			终端安装
systemctl start firewalld			启动
systemctl disable firewalld		停止
systemctl stop firewalld			禁用
~~~

命令格式
> firewalld -cmd [选项 ...]

通用选项
> -h, --help			显示帮助信息
> -V, --version			显示版本信息
> -q, --quiet			不打印状态信息

状态选项
> --state				显示firewalld状态
> --reload				不中断服务器重新加载
> --complete-reload				中断所有连接的重新加载
> --runtime-to-permanent		将当前防火墙规则永久保存
> --check-config				检查配置正确性

日志选项

> --get-log-denied				获取记录被拒绝的日志

配置firewalld
~~~
firewall-cmd	--get-active-zones			查看区域信息
firewall-cmd	--panic-on			拒绝所有包
firewall-cmd	--panic-off		取消拒绝状态
firewall-cmd --query-panic			查看是否拒绝

firewall-cmd	--reload			更新防火墙规则

firewall-cmd	--enable service=ssh			允许ssh服务通过
firewall-cmd	--disable service=ssh			禁止ssh服务通过
firewall-cmd --list-services			显示当前服务
~~~