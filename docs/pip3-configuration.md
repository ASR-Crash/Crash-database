## pip3安装

### Windows

https://bootstrap.pypa.io/get-pip.py

文本另存为get_pip.py： [get-pip.py](get-pip.py) 

cmd执行：

		python get-pip.py

### Linux
安装：

		sudo apt install python3-pip 

更新：

		sudo pip3 install --upgrade pip

## pip换源

单次使用：

		pip install xxx -i  https://pypi.tuna.tsinghua.edu.cn/simple/

永久修改：

- ####  WIN10:


		新建 %HOMEPATH%\pip\pip.ini

 [pip.ini](pip.ini) 

		[global]
		index-url = https://pypi.tuna.tsinghua.edu.cn/simple
		
		[install]
		trusted-host = https://pypi.tuna.tsinghua.edu.cn
- #### LINUX:


		新建 ~/.pip/pip.conf 


		[global]
		index-url = https://pypi.tuna.tsinghua.edu.cn/simple
	
		[install]
		trusted-host = https://pypi.tuna.tsinghua.edu.cn

---

## pip升级python库

		pip list --outdated

- 升级单个		

		pip install --upgrade
	
- 批量升级

		pip install pip-review
		pip-review --local --interactive
