## ADB（Android调试桥）

### 卸载安卓系统软件

1. 多次快速点击版本号，进入开发者模式
2. 进入开发人员选项，开启USB调试，USB弹出提示，监控ADB安装应用，仅充电下允许ADB调试
3. 下载ADB Kits [Downloads - ADB Shell](https://adbshell.com/downloads)
4. 通过cmd打开adb.exe，手机连接到电脑
5. 输入 adb device 查看 list of devices attached 是否有device
6. 输入adb shell 进入调试
		
		pm list packages -s  #system apps
		pm list packages -3  #third-party apps
		pm uninstall -k --user 0 <name of package>
		
		for example:
		pm uninstall -k --user 0 com.android.mediacenter

7. done！
