# Mac终端常用命令
### 基本命令
* 如果出现`Permission denied`，可使用`chmod +x <file.sh>`或者` chmod 777 <file.sh>`来获得权限后，再重试

* `chmod +x`和`chmod 777`可以将文件转换为双击可执行的文件，这样就可以把文件变成默认终端打开，前提是**不能**`touch <file>`时给file命名带有后缀
* 列出文件：`ls`
* 转换目录：`cd xxx/xxx`
* 建立新目录：`mkdir <dir name>`
* 拷贝文件：`cp 参数 源文件 目标`，如`cp -R /path/x.md /System/Library/Extensions`（参数R表示对目录进行递归操作）
* 删除文件：`rm 参数 文件`，如`rm -rf /path/x.md`，**参数－rf 表示递归和强制，千万要小心使用，如果执行了 rm -rf / 你的系统就全没了**。
* 重命名文件：`mv 旧文件名 新文件名`
* 文本编辑：`nano 文件名`
* 在finder中打开当前目录：`open .`
* 查看man手册(manual)：`man <any command name>`
* 在pdf中查看man手册：`man cal <any command name> | open -a Preview -f`
* 打印当前目录所有文件夹占空间大小：`du -sh *`
* 查找目录下的apk文件，也可以是其他文件：`find <dir>/ -name *.apk`
* 创建文件：`touch <file>`
* 创建文件并输入数据：`echo 'test' > test.md`
* 查看IP：`ifconfig`或`ifconfig en0`
* 检查根目录的文件夹大小：`du -sh *`可以查看，删除过大不必须的文件夹
* 打印目录tree型结构：`find . -print | sed -e 's;[^/]*/;|____;g;s;____|; |;g'`**（但是）我无法指定打印层级**
* 可以使用工具`tree`打印目录tree型结构（可以指定层级）：`tree -L 3`，如果中文乱码，可以使用`tree -N -L -3`

### 解压zip
语法：unzip [options] 压缩文件名.zip，具体跟多的参数可以直接执行"unzip"查看

常用options的含义分别为： 
-x ：文件列表解解压缩文件，但不包括指定的file文件。 
-v ：查看压缩文件目录，但不解压。 
-t ：测试文件有无损坏，但不解压。 
-d ：目录 把压缩文件解到指定目录下。 
-z ：只显示压缩文件的注解。 
-n ：不覆盖已经存在的文件。 
-o ：覆盖已存在的文件且不要求用户确认。 
-j ：不重建文档的目录结构，把所有文件解压到同一目录下。 

* `unzip <name>.zip` 解压到当前目录
* `unzip -n <name>.zip -d <floder>` 解压到folder目录下，如果已存在解压目录则不覆盖
* `unzip -v <name>.zip` 查看zip文件，但不解压

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
* [mac 终端 常用命令](http://www.cnblogs.com/iphone520/archive/2012/03/26/2418468.html)
* [mac 下的 tree 命令 终端展示你的目录树结构](http://yijiebuyi.com/blog/c0defa3a47d16e675d58195adc35514b.html)