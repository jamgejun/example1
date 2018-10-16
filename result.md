git init 初始化以git管理的仓库

git status 查看暂存区状态

git add file 添加文件到暂存区

git commit -m "" 提交暂存区文件到版本库，并附加msg

git diff file 查看版本库文件和当前修改文件的不同

git log 查看暂存区提交日志

git reset --hard HEAD^ 回退到上一版本

git reset --hard version 回到目标版本号

git reflog 查看版本号

git checkout -- file 撤销更改
（当文件已经在暂存区时，会将暂存区文件覆盖当前工作区文件）
（当文件没有到暂存区时，会将版本库文件覆盖当前工作区文件）

git remote add origin "adress".git 将github仓库和本地仓库合并

git push -u master 将master分支版本库内容提交到github远程仓库
（由于远程库是空的，我们第一次推送master分支时，加上了 –u参数，Git不但会把本地的master分支内容推送的远程新的master分支，还会把本地的master分支和远程的master分支关联起来，在以后的推送或者拉取时就可以简化命令。）

git merge branchName 将目的分支的内容合并到当前分支