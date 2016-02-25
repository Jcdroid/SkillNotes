# Git笔记

初始化：`git init`

添加远程仓库：`git remote add origin <url>`

移除已添加远程仓库：`git remote set-url origin <url>`

克隆远程仓库：`git clone <url>`

添加所有文件：`git add *`

从本地仓库移除文件夹：`git rm -r --cached <floder>`

移除文件：`git rm <file>`

添加提http://stackoverflow.com/questions/115983/how-can-i-add-an-empty-directory-to-a-git-repository交文件到本地仓库：`git commit -m "message"`

从本地仓库push文件到远程主仓库：`git push origin master`

从远程主仓库pull文件到本地仓库：`git pull origin master`

查看commit日志：`git log`

查看仓库状态：`git status`

查看修改：`git diff`

忽略文件和文件夹：新建`.gitignore`（windows中需要创建时使用.gitignore.后面加一个.才不会报不能存在空名字的问题），然后添加忽略文件和文件夹的路径，如果想忽略文件夹下面的所有文件和文件夹，但是同时想保存这个文件夹，这时就需要在这个文件夹下面新建.gitkeep文件(1)



### 参考

1. [How can I add an empty directory to a Git repository? -> Mark Amery](http://stackoverflow.com/questions/115983/how-can-i-add-an-empty-directory-to-a-git-repository)
2. [Git教程](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000)