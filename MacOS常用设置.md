# Mac常用设置

### Finder
* **打开文件夹终端**：在`系统偏好设置` - `键盘` - `快捷键` - `服务`中，勾选上`新建位于文件夹位置的终端窗口`。
* **快速查找文件或文件夹**：打开`Spotlight`（`ctrl`+空格）。
* **设置Finder打开指定文件夹**：打开Finder后，点击`Finder` - `偏好设置` - `通用` - `开启新Finder窗口时打开`选择需要指定的目录。
* 单引号和双引号的问题：在`系统偏好设置` - `键盘` - `文本`中，选择需要的智能引号样式。
* **修改Mac软件Command+Q退出快捷键（防止误触）**：`系统偏好设置` - `键盘` - `快捷键` - `应用程序快捷键`，添加对应的应用退出的快捷键（如Chrome：选择Google Chrome，编辑菜单标题：退出Google Chrome，编辑快捷键，添加）。
* **添加三指拖移**：`系统偏好设置` - `辅助功能` - `鼠标与触控板` - `触控板选项`，勾选启用拖移，选中三指拖移。
* **调整显示器颜色**：`系统偏好设置` - `显示器设置` - `普通RGB颜色`

### 删除GarageBand
```
rm -rf /Library/Application\ Support/GarageBand
rm -rf /Library/Application\ Support/Logic
rm -rf /Library/Audio/Apple\ Loops
```

### 常见问题
* 出现不能打开图片，并且弹出提示需要权限
> 重启电脑即可



### 参考
* [10 个实用技巧，让 Finder 带你飞](http://sspai.com/27403/)
* [Mac中的garageband如何完全删除？](https://www.zhihu.com/question/48348923/answer/121311324)