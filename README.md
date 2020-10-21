# awesome-guide
awesome-guide


### mac
https://support.apple.com/zh-cn/HT201834
--断开显示器或投影仪的连接
在断开显示器或投影仪的连接之前，请将 Mac 置于睡眠状态。
选取苹果 () 菜单 >“睡眠”，然后断开显示器或投影仪的连接。

--mac 查看硬盘使用量 （需安装 smartctl）
smartctl -a /dev/disk0  

--mac 10.15 升级后 无法写入/data文件
sudo mount -uw /
sudo chmod 777 /data
```
1、重启mac，按住`Command+R`，等到系统进入安全模式。
2、选择一个账户，然后点击屏幕上方的工具栏找到命令行工具。
3、执行，命令`csrutil disable`
4、重启电脑后，不要进入安全模式，执行命令`sudo mount -uw /`
5、执行命令 `sudo mkdir /data`
6、执行命令 `sudo chmod 777 /data`
7、重启电脑，进入安全模式，执行命令 `csrutil enable` （开启SIP）
```


debug
step over
step into
force step into
step out

AppResponse


