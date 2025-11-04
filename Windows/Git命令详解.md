# Git命令详解

```shell
git init	
	初始化仓库，在当前目录新建一个Git代码库，基本上是创建一个具有`objects`，`refs/head`，`refs/tags`和模板文件的`.git`目录

git config
    git config -- list  显示当前的配置
    git config [--global] user.name "[name]"   设置提交信息时的用户名
    git config [--global] user.email "[email address]"  设置提交信息是的邮箱

git add
	git add [file1] [file2] ...		添加指定文件到暂存区
	git add [dir]	添加指定目录到暂存区，包括子目录
	git add .	添加当前目录的所有文件到暂存区
	
git commit
	git commit -m [message]		把暂存区的文件提交到仓库区
	git commit [file1] [file2] ... -m [message]	提交暂存区的指定文件到仓库区
	git commit -a	提交工作区自上次commit之后的变化，直接到仓库区

git status
	显示有变更的文件
	
git remote
	git remote -v	显示所有远程仓库
	git remote add <name> <git-repo-url>	关联远程仓库
	# 例如 git remote add origin https://github.com/xxxxxx # 是远程仓库的名称，通常为 origin 
	
git pull
	git pull [remote] [branch]	取回远程仓库的变化，并与本地分支合并
	git push [remote] [branch]	上传本地指定分支到远程仓库
	git push [remote] --force	强行推送当前分支到远程仓库，即使有冲突
	
```



