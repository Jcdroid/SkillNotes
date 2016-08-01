# Mac终端常用命令
### 基本命令
* 列出文件：`ls`
* 转换目录：`cd xxx/xxx`
* 建立新目录：`mkdir <dir name>`
* 拷贝文件：`cp 参数 源文件 目标`，如`cp -R /path/x.md /System/Library/Extensions`（参数R表示对目录进行递归操作）
* 删除文件：`rm 参数 文件`，如`rm -rf /path/x.md`，**参数－rf 表示递归和强制，千万要小心使用，如果执行了 rm -rf / 你的系统就全没了**。
* 移动文件：`mv 源文件 目标`
* 文本编辑：`nano 文件名`
* 在finder中打开当前目录：`open .`
* 查看man手册：`man <any command name>`
* 在pdf中查看man手册：`man cal <any command name> | open -a Preview -f`

### 目录操作
|命令名|功能描述|举例|
|---|---|---|
|mkdir|创建一个目录|mkdir dir|
|rmdir|删除一个目录|rmdir dir|
|mvdir|移动或重命名一个目录|mvdir dir1 dir2|
|cd|改变当前目录|cd dir|
|pwd|显示当前目录的路径名|pwd|
|ls|显示当前目录的内容|ls -la|

### 文件操作
|命令名|功能描述|举例|
|---|---|---|
|cat|显示或连接文件|cat filename|
|cp|复制文件或目录|cp file1 file2|
|rm|删除文件或目录|rm filename|
|mv|改变文件名或所在目录|mv file1 file2|

### 参考
[mac 终端 常用命令](http://www.cnblogs.com/iphone520/archive/2012/03/26/2418468.html)