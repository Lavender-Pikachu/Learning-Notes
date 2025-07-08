# Git
## 背景
备份
    A负责的模块就要完成了，就在即将Release之前的一瞬间，电脑突然蓝屏，硬盘损坏！！！几个月的努力付之东流

代码回滚
    项目中需要添加很复杂的功能，B摸索了一个星期终于有眉目了，可是这被改得面目全非的代码已经回不到从前。
协同开发
    A和B先后从文件服务器上下载了同一个问题间:Analysis.java。A在Analysis.java文件中第30行声明了一个方法：count(),先保存到文件服务器上；B在Analysis,java文件中的第50行声明了一个方法sum(),也随后保存到文件服务器上，于是count()方法就只存在于A的记忆中了
追溯问题代码的编写人和编写时间 

## 版本控制方式
SVN
Git

## Git Architecture


- 工作区
- 暂存区
- 本地仓库
- 远程仓库

## git common command
|command| description|
|------- |---------|
|git init .| 在当前目录初始化一个新的Git仓库  |
|git status| 查看已修改但未暂存、暂存但未提交的文件 |
|git branch| 查看当前工作所在的分支|
|git checkout <branch_name>|切换到其他分支|
|git checkout -b <new_branch_name>| 创建并切换到一个新分支|
|git add <file_name1> <fil1_name2>| 将指定修改的文件添加到暂存区|
|git add .| 添加所有修改的文件到暂存区|
|git commit -m "<description>"| 提交暂存区的文件到本地仓库，添加描述内容|
|git log|查看当前分支的提交历史|
|git diff|查看尚未暂存的文件差异|
|git checkout -- <file_name>|撤销对文件的修改(未提交前)|
|git remote add origin <remote_repo_url>|将远程仓库添加到本地仓库|
|git remote -v| 查看当前仓库远程仓库的信息|
|git push origin <branch_name>| 将本地提交推送到远程仓库|
|git pull origin <branch_name>|从远程仓库拉取最新的更改，并合并到当前分支|
|git push --force origin <branch_name>|强制将本地分支推送到远程仓库，覆盖远程仓库的内容|
|git push origin --delete <branch_name>|删除远程仓库中的分支|
|git clone <remote_repo_url>|克隆一个远程仓库到本地|
|git branch -a |查看所有本地和远程分支|
|git branch -d <branch_name>|删除本地的分支(强制删除使用-D)|
|git merge <branch_name>|讲一个分支合并到当前分支|
|git tag <tag_name>| 在当前提交出创建一个标签|
|git tag|查看所有的标签|
|git push origin <tag_name>|将本地标签推送到远程仓库|
|git tag -d <tag_name>| 删除本地标签|
|git config --global user.name "Your Name"||
|git config --global user.email "your_email@example.com"
|git config -list||
|git push origin --delete <tag_name>|删除远程标签|
|git config --edit| 查看当前Git配置的文件位置|
|git clean -fd|删除未跟踪的文件和目录|