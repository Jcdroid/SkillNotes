# Chrome打包插件流程

### 打包本地扩展

在文件浏览器中打开`C:\Users\<username>\AppData\Local\Google\Chrome\User Data\Default\Extensions`，在chrome中找到对应插件的hash值，点击`打包扩展程序`即可

### 加载本地扩展

打开chrome的扩展程序列表，~~直接将打包出来的crx文件拖进去即可~~，不能使用拖拽，否则会出现`此扩展可能已经损坏`的错误，需要把crx改为rar后，解压，再使用`加载已解压的扩展程序`即可



### 参考

* [[chrome插件提示已损坏怎么办？解决此扩展程序可能已损坏安装方法](http://www.cnplugins.com/tool/chajiasunhuai.html)](http://www.cnplugins.com/tool/chajiasunhuai.html)

* [【已解决】怎么从Chrome浏览器中导出扩展程序为crx文件？](http://www.cnplugins.com/tool/export-cnplugins-crx.html)