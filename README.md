# GIT
## 1.创建本地代码库
    $ git init                      新建本地仓库
    $ git clone [url]               从远程仓库克隆

## 2.配置
    $ git config                    显示git配置
    $ git config -e [--global]      编辑git配置文件
    $ git config [--global] user.name "username"    设置提交代码是的用户名
    $ git config [--global] user.email "email address"      设置提交代码是的用户邮箱

## 3.增加/删除
    $ git add [file1]     添加指定文件到暂存区
    $ git add .           添加所有文件到暂存区
    $ git rm [file1] [file2]        删除暂存区指定文件

## 4.提交代码
    $ git commit -m [message]   提交缓存区到仓库
    $ git commit [file1] [file2] -m [message]   添加指定文件到仓库区
    $ git commit -a     提交工作区自上次commit之后的变化直接到仓库区

## 5.分支
    $ git branch    列出所有分支
    $ git branch -r    列出所有远程分支
    $ git branch -a    列出远程、本地所有分支
    $ git branch [newBranch]    新建分支
    $ git checkout -b [newBranch]   新建并切换到该分支上
    $ git checkout [branch]     切换到指定分支
    $ git checkout -    切换到上一分支

## 6.同步
    $ git remote update     更新远程仓库
    $ git fetch [remote]    下载远程仓库的所有改动
    $ git remote add [shortName] [url]  增加一个新的远程仓库
    $ git fetch     从远程获取更新到本地
    $ git pull      从远程获取更新到本地并merge到本地
    $ git push origin [branche]     推送到指定分支，默认master分支

## 7.连接
    $ git remote add origin [url]   本地仓库与远程仓库建立连接
    $ git push -u origin master     推送到远程仓库并于远程仓库的master分支建立连接
    $ git remote rm origin      删除本地仓库与远程仓库的连接