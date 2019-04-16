# Mac常用设置

##### 绿豆沙色值
* RGB: R(199)、G(237)、B(204)
* HSB: H(85)、S(123)、B(205)
* HEX: `#C7EDCC`

### Finder
* **打开文件夹终端**：在`系统偏好设置` - `键盘` - `快捷键` - `服务`中，勾选上`新建位于文件夹位置的终端窗口`。

* **快速查找文件或文件夹**：打开`Spotlight`（`ctrl`+空格）。

* **显示隐藏文件快捷键**：在 macOS Sierra及以上(Mojave)，我们可以使用快捷键 ⌘⇧.(Command + Shift + .) 来快速（在 Finder 中）显示和隐藏隐藏文件了。获取使用命令行
	```
  //显示隐藏文件
  defaults write com.apple.finder AppleShowAllFiles -bool true
  //不显示隐藏文件
  defaults write com.apple.finder AppleShowAllFiles -bool false
  ```
最后重启Finder。

* **设置Finder打开指定文件夹**：打开Finder后，点击`Finder` - `偏好设置` - `通用` - `开启新Finder窗口时打开`选择需要指定的目录。

* 单引号和双引号的问题：在`系统偏好设置` - `键盘` - `文本`中，选择需要的智能引号样式。

* **修改Mac软件Command+Q退出快捷键（防止误触）**：`系统偏好设置` - `键盘` - `快捷键` - `应用程序快捷键`，添加对应的应用退出的快捷键（如Chrome：选择Google Chrome，编辑菜单标题：退出Google Chrome，编辑快捷键，添加）。

* **添加三指拖移**：`系统偏好设置` - `辅助功能` - `鼠标与触控板` - `触控板选项`，勾选启用拖移，选中三指拖移。

* **调整显示器颜色**：`系统偏好设置` - `显示器设置` - `普通RGB颜色`

* **查看IP地址**：终端运行`ifconfig`

* **终端欢迎页自定义**：终端输入`cd /etc`，再输入`sudo pico motd`，然后在其中输入你想显示在终端欢迎页的内容（可以在[这里](http://www.asciiworld.com/)找到字符图形），最后 control + x，输入 y 保存，重启终端就可以看到新的欢迎页。

  ```
  	 ___________________________
      !\_________________________/!
      !!                         !!
      !! C:\> _                  !!
      !!                         !!
      !!                         !!
      !!                         !!
      !!_________________________!!
      !/_________________________\!
         __\_________________/__/!_
      ________________________    (__
     /oooo  oooo  oooo  oooo /!   _  )_
    /ooooooooooooooooooooooo/ /  (_)_(_)
   /ooooooooooooooooooooooo/ /    (o o)
  /C=_____________________/_/    ==\o/==
  ```

### Mac系统占用存储太多
##### 删除GarageBand
```
rm -rf /Library/Application\ Support/GarageBand
rm -rf /Library/Application\ Support/Logic
rm -rf /Library/Audio/Apple\ Loops
```

##### 检查根目录的文件夹大小
在终端使用`du -sh *`可以查看，删除过大不必须的文件夹

### 常见问题
* 出现不能打开图片，并且弹出提示需要权限

	> 重启电脑即可
* 如果出现外接机械键盘和普通按键不一样的情况，可以去设置页面更改键盘类型


### 参考
* [10 个实用技巧，让 Finder 带你飞](http://sspai.com/27403/)
* [Mac中的garageband如何完全删除？](https://www.zhihu.com/question/48348923/answer/121311324)