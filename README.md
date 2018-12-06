# GIT
##1.创建本地代码库
    $ git init                      新建本地仓库<br />
    $ git clone [url]               从远程仓库克隆<br />

##2.配置
    $ git config                    显示git配置<br />
    $ git config -e [--global]      编辑git配置文件<br />
    $ git config [--global] user.name "username"    设置提交代码是的用户名<br />
    $ git config [--global] user.email "email address"      设置提交代码是的用户邮箱<br />

##3.增加/删除
    $ git add [file1]     添加指定文件到暂存区<br />
    $ git add .           添加所有文件到暂存区<br />
    $ git rm [file1] [file2]        删除暂存区指定文件<br />

##4.提交代码
    $ git commit -m [message]   提交缓存区到仓库<br />
    $ git commit [file1] [file2] -m [message]   添加指定文件到仓库区<br />
    $ git commit -a     提交工作区自上次commit之后的变化直接到仓库区<br />

##5.分支
    $ git branch    列出所有分支<br />
    $ git branch -r    列出所有远程分支<br />
    $ git branch -a    列出远程、本地所有分支<br />
    $ git branch [newBranch]    新建分支<br />
    $ git checkout -b [newBranch]   新建并切换到该分支上<br />
    $ git checkout [branch]     切换到指定分支<br />
    $ git checkout -    切换到上一分支<br />

##6.同步
    $ git remote update     更新远程仓库<br />
    $ git fetch [remote]    下载远程仓库的所有改动<br />
    $ git remote add [shortName] [url]  增加一个新的远程仓库<br />
    $ git fetch     从远程获取更新到本地<br />
    $ git pull      从远程获取更新到本地并merge到本地<br />
    $ git push origin [branche]     推送到指定分支，默认master分支<br />