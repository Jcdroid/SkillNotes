# cURL常用命令

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