## Git使用

> 初始化

		git init

> 添加文件

		git add .

> 查看状态

		git status

> 添加至仓库

		git commit -m 'description'

>关联远程服务器

		git remote add origin [git-url]

>查看远程服务器信息

		git remote -v
		git remote show origin      

>本地上传文件至远程

		git push
		git push origin [branch-name]
		git push -u origin [branch-name](创建)

>远程拉取文件至本地

		git pull

> 创建分支

		git branch [branch-name]

>切换分支

		git checkout [branch-name]

>合并至当前分支

		git merge [branch-name]

>恢复最近一次提交

		git reset --hard

---

## Debug

> warning: LF will be replaced by CRLF

		git config --global core.autocrlf false

> fatal: The current branch master has no upstream branch

		git push -u origin master

> fatal: Could not read from remote repository

Local:

		ssh-keygen -t rsa -C "youremail@example.com"
		eval "$(ssh-agent -s)"
		ssh-add ~/.ssh/id_rsa

GitHub:

		Settings–>SSH and GPG keys–>New SSH key
		input code in: id_rsa.pub

验证：

		ssh -T git@github.com

Failed to connect to github.com port 443 after 21098 ms: Timed out：

		git config --global https.proxy
		git config --global --unset https.proxy