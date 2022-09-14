# Cmder


## 安装
[Cmder | Console Emulator](https://cmder.app/)

在环境变量添加Cmder.exe的路径

## 右键配置

管理员身份打开cmd：

		Cmder.exe /REGISTER ALL

## 更改命令行

打开Setting：

		win+alt+p

选择command line:

		bash -cur_console:p

![Cmder-startup](Cmder-startup.png)

## 修改命令提示符
路径：

		cmder\vendor\clink.lua

修改：

		local lambda = "[anything you want]"

![Cmder-prompt](Cmder-prompt.png)

## 快捷键

		Ctrl+T：新页签
		Ctrl+W：关闭页签
		Ctrl+Tab：切换页签
		Ctrl+1：切换到第1个页签
		Ctrl+n：切换到第n个页签
		Ctrl+r：历史命令搜索
		Alt+Shift+1：cmd管理员模式
		Alt+Shift+2：cmd
		Alt+Shift+3：powershell管理员模式
		Alt+Shift+4：powershell
		Alt+Enter：切换全屏
		Alt+F4：关闭所有页签
