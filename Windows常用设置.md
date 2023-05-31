# Windows常用设置

##### 绿豆沙色值

- RGB: R(199)、G(237)、B(204)
- HSB: H(85)、S(123)、B(205)
- HEX: `#C7EDCC`

### Tips
* 删除github登录账号等账号密码操作：`控制面板\用户帐户和家庭安全\凭据管理器`，删除对应的凭据即可

### Windows 10激活
* win10 G版激活方法如下：
	```
	在命令提示符（管理员）下运行下面的指令
	slmgr /ipk YYVX9-NTFWV-6MDM3-9PT4T-4M68B
	slmgr /skms kms.03k.org
	slmgr /ato
	```

###  Windows 11右键默认显示更多选项
> 执行完命令后，不需要重启电脑，重启资源管理器即可，用命令：`taskkill /f /im explorer.exe & start explorer.exe`

- 开启更多选项（管理员运行命令）：`reg.exe add "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /f /ve`
- 回复默认选项（管理员运行命令）：`reg.exe delete "HKCU\Software\Classes\CLSID\{86ca1aa0-34aa-4e8b-a509-50c905bae2a2}\InprocServer32" /va /f`

### 常见问题
