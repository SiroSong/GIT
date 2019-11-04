# GIT
## 1.创建本地代码库

> 新建本地仓库

    $ git init                      

> 从远程仓库克隆

    $ git clone [url]               

## 2.配置

> 显示git配置

    $ git config                    

> 编辑git配置文件

    $ git config -e [--global]      

> 设置提交代码是的用户名

    $ git config [--global] user.name "username"    

> 设置提交代码是的用户邮箱

    $ git config [--global] user.email "email address"      
## 3.增加/删除

> 添加指定文件到暂存区

    $ git add [file1]     

> 添加所有文件到暂存区

    $ git add .           
 
> 删除暂存区指定文件 
 
    $ git rm [file1] [file2]        

## 4.提交代码

> 提交缓存区到仓库

    $ git commit -m [message]   

> 添加指定文件到仓库区

    $ git commit [file1] [file2] -m [message]   

> 提交工作区自上次commit之后的变化直接到仓库区

    $ git commit -a     
## 5.分支

> 列出所有分支

    $ git branch    

> 列出所有远程分支

    $ git branch -r    

> 列出远程、本地所有分支

    $ git branch -a    

> 新建分支

    $ git branch [newBranch]    

> 新建并切换到该分支上

    $ git checkout -b [newBranch]  

> 切换到指定分支

    $ git checkout [branch]     

> 切换到上一分支

    $ git checkout -

> 删除本地分支

    $ git branch -D [branch]

> 删除远程分支

    $ git branch -r -d origin/branch-name   // 删除了本地的远程分支跟踪
    $ git push origin :branch-name    //删除远程分支

## 6.同步

> 更新远程仓库

    $ git remote update  

> 下载远程仓库的所有改动

    $ git fetch [remote]    下载远程仓库的所有改动

> 增加一个新的远程仓库

    $ git remote add [shortName] [url]  

> 从远程获取更新到本地

    $ git fetch     

> 从远程获取更新到本地并merge到本地

    $ git pull      

> 推送到指定分支，默认master分支

    $ git push origin [branche]     

> 创建并拉取远程分支

    $ git checkout -b [newbranch] origin/[remotebranch] 

#### or  

    $ git checkout -b [newbranch]
    $ git pull origin [remotebranch]
    
> 创建并推送之远程分支    

    $ git checkout -b [newbranch]
    $ git pull origin [remotebranch]
    
> 远程分支覆盖本地分支   

    $ git fetch --all
    $ git reset --hard origin/[remotebranch]
    $ git pull

## 7.连接
> 本地仓库与远程仓库建立连接

    $ git remote add origin [url]  

> 推送到远程仓库并于远程仓库的master分支建立连接

    $ git push -u origin master  

> 删除本地仓库与远程仓库的连接

    $ git remote rm origin      

## 8.冲突

> 多人协同, 本地线上代码同步并处理可能出现的冲突

    $ git stash
    $ git pull
    $ git stash pop

## 9.追踪

> 推送时为本地分支建立远程分支追踪

    $ git push --set-upstream origin [branch_name]

> 为本地分支建立远程分支追踪

    $ git branch --set-upstream-to=origin/[branch_name] feature-expert