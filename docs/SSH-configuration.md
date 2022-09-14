## Ubuntu安装SSH

1、查看已安装服务

		dpkg -l | grep ssh

2、安装未安装服务

		sudo apt install openssh-server
		sudo apt install openssh-client

3、查看ssh-server是否启动

		ps -e | grep ssh

4、配置ssh_config

		sudo nano /etc/ssh/ssh_config


		cancel the # before: 
		# PasswordAuthentication yes

5、配置sshd_config

		sudo nano /etc/ssh/sshd_config


		PermitRootLogin prohibit-password
		change into:
		PermitRootLogin yes

6、重启ssh服务，Done

		sudo /etc/init.d/ssh restart