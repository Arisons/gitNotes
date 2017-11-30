# git使用大全
### 1、git 初始化
## 小结：
初始化一个git仓库，使用<font style="color:red">`git init`</font>命令。
添加文件到git仓库，分两步：

1、使用命令<font style="color:red;">` git add 文件` </font>（文件add去到了本地暂存区）
2、使用命令<font style="color:red;">`git commit -m '提交信息内容'`</font>（将暂存区的文件提交到分支）

### 2、版本回退

## 小结：

HEAD指向的版本就是当前版本，因此，git允许我们在版本的历史之间穿梭，使用命令 <font style="color:red;">`git reset --hard commit_id `</font>

果然回退到上一版本 可以使用命名 <font style="color:red;">`git reset --hard HEAD^`</font>

回退到上上版本 <font style="color:red;">`git reset --hard HEAD^^`</font>，当然往上100个版本写100个<font style="color:red;">`^`</font>是不显示的，所以可以写成<font style="color:red;">`HEAD~100`</font>

### 3、撤销修改

## 小结：

<font style="color:red;">`git checkout --file`</font>命令中的<font style="color:red;">`--`</font>很重要，没有<font style="color:red;">`--`</font>，就变成了“`切换到另一个分支`”的命令。

场景1：当你该乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令<font style="color:red;">`git checkout --file`</font>。

场景2：当你补单改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令<font style="color:red;">`git reset HEAD file`</font>,就回到了场景1，第二步按场景1操作。

### 4、删除文件

## 小结：

<font style="color:red;">`git rm file`</font> 用于删除一个文件

### 5、远程仓库

## 小结：






