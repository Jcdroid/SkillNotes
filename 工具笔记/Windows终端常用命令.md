# Windows终端常用命令
### 基本命令
* `explorer .` 在explorer打开当前路径
* `echo %path%` 可以查看配置的环境变量path
* 打印目录tree型结构：windows中默认带有tree命令，可以输入`tree /?`查看帮助信息
* 将tree输入结果写入文件：`tree /F >tree.txt`

### 文件操作

###　目录操作

### 端口占用问题
1. 根据端口号查找对应的进程号：`netstat -ano | findstr 8081`(或者80，会查看所有有80的tcp、udp连接)，最后一位是PID
2. 据进程号寻找进程名称：`tasklist | findstr 10048`

### 常见问题
* ping、tree等系统命令不能正常使用

	由于在环境变量path中没有配置`C:\Windows\System32`导致的，在path中追加`C:\Windows\System32`即可

* explorer命令不能正常使用

	由于环境变量中没有配置`C:\Windows\SysWOW64;`导致的，在path中追加`C:\Windows\SysWOW64`即可

	> 具体哪个命令不能使用，可以在`everything`中搜索`xxx.exe`，如`explorer.exe`，然后把其路径配置到path中

* Windows cmd不能执行shell脚本的问题
	
	可以使用`git bash`执行shell脚本

### 参考