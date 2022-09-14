## 树莓派配置

打开终端

	Ctrl+Alt+t

打开配置

	sudo raspi-config

关机/重启

	shutdown -h -t 0
	sudo reboot

更新

	sudo apt-get update
	sudo apt-get upgrade

自启动程序配置：

1. 在/home/pi/.config文件夹里新建autostart文件夹（已有可忽略）

		pi@raspberry:~ $ mkdir .config/autostart

2. 在autostart里新建desktop文件（名字随意，后缀必须为.desktop)

		pi@raspberry:~ $ nano .config/autostart/testboot.desktop

3. desktop文件内容

		[Desktop Entry]
		Type=Application
		Exec=/home/pi/... （指定文件的全部途径）

开启ssh

	sudo systemctl enable ssh 
	sudo systemctl start ssh

查看IP

	hostname -I

检测USB设备

	lsusb

查看摄像头设备文件

	ls/dev/video*

视频VNC界面

	sudo apt-get install luvcview
	luvcview -s 1920X1080

远程桌面

	sudo apt-get install xrdp
	sudo service xrdp restart
	ifconfig

获取温度

	cd /sys/class/thermal/thermal_zone0
	cat temp

取消鼠标显示

	sudo nano /etc/lightdm/lightdm.conf 
	#xserver-command=X 修改为：
	xserver-command=X -bs -core -nocursor