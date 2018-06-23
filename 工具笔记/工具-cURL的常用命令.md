# cURL常用命令

	-X/--request [GET|POST|PUT|DELETE|…]  使用指定的http method發出 http request
	-H/--header                           設定request裡的header
	-i/--include                          顯示response的header
	-d/--data                             設定 http parameters 
	-v/--verbose                          輸出比較多的訊息
	-u/--user                             使用者帳號、密碼
	-b/--cookie                           cookie  

### 发送GET、POST请求
* 使用curl发送GET请求：`curl protocol://address:port/url?args`
* 使用curl发送POST请求：`curl -d "args" protocol://address:port/url`

### 其他

* `curl https://www.baidu.com` 下载单个文件，默认将输出打印到标准输出中(STDOUT)中

* `curl -o test.html http://www.baidu.com/gettext.html` 通过-o/-O选项保存下载的文件到指定的文件中
* `curl -O URL1 -O URL2` 同时获取多个文件
* 默认curl使用GET方式请求数据，这种方式下直接通过URL传递数据
可以通过 --data/-d 方式指定使用POST方式传递数据

	```
	# GET
	curl -u username https://api.github.com/user?access_token=XXXXXXXXXX
	
	# POST
	curl -u username --data "param1=value1&param2=value" https://api.github.com
	
	# 也可以指定一个文件，将该文件中的内容当作数据传递给服务器端
	curl --data @filename https://github.api.com/authorizations
	```
除了使用GET和POST协议外，还可以通过 -X 选项指定其它协议，如：
`curl -I -X DELETE https://api.github.cim`
* `curl --form "fileupload=@filename.txt" http://hostname/resource` 上传文件

### 参考
* [CURL常用命令](https://www.cnblogs.com/gbyukg/p/3326825.html)
* [curl网站开发指南](http://www.ruanyifeng.com/blog/2011/09/curl.html)
* [使用curl指令測試REST服務](http://ju.outofmemory.cn/entry/84875)