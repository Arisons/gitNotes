## git 常用命令
### git 常用操作命令收集：

#### 1)远程仓库相关命令
检出仓库：git clone XXXXX

查看远程仓库：git remote -v

删除远程仓库：git remote rm [name]

修改远程仓库：git remote set-url --push[name][url]

拉取远程仓库：git pull [remoteName][localBranchName]

推送远程仓库：git push [remoteName][lacalBranchName]

#### 2）分支（branch）操作相关命令

查看本地分支：git branch

查看远程分支：git branch -r

创建本地分支： git branch [name]

切换分支：git checkout [name]

创建新分支并立即切换到新分支：git checkout -b [name]

删除分支：git branch -d [name]  ----d选项只能删除已经参与了合并的分支，对于未有合并的分支是无法删除的。如果想强制删除一个分支，可以使用-D选项

创建远程分支(本地分支push到远程)：$ git push origin [name]

git push origin [name]:master //提交远程分支作为远程master分支

git push origin test:test //提交本地test分支作为远程test分支


#### 版本tag操作命令

查看版本：git tag

创建版本：git tag [name]

删除版本：git tag -d [name]

#### 3)忽略一些文件、文件夹不提交

在仓库根目录下创建名称为：'.gitignore'的文件，写入不需要的文件夹名或者文件，每个元素占一行即可，如

target

bin

*.db


新建本地分支后将本地分支推送到远程库, 使用git pull 或者 git push 的时候报错

`gitThere is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> merged0.9.6`

是因为本地分支和远程分支没有建立联系  (使用git branch -vv  可以查看本地分支和远程分支的关联关系)  .根据命令行提示只需要执行以下命令即可
git branch --set-upstream-to=origin/远程分支的名字 本地分支的名字  

 

## 关于git 生成多个ssh key 管理问题

参考：
`http://www.jianshu.com/p/f7f4142a1556`






