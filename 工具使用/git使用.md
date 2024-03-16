## Git工具的使用

#### 基本用法

```shell
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/xxxx/xx.git
git push -u origin main
```

> 这是Github官方给出的git提交代码方式，下面逐步介绍每条命令的用途

* `git init` 在本目录下创建.git文件夹，用于存放git的相关文件。
* `git add README.md` 在**暂存区**添加目录下的README.md。
* `git commit -m "first commit" `在本地仓库提交**暂存区**的文件，`-m`后为commit的message。
* `git branch -M main` 将主分支重命名为main(*默认为master*，这是一项github的新改变)。
* `git remote add origin https://github.com/xxxx/xx.git`将远程仓库连接至本地仓库，并且用origin来命名远程仓库。
* `git push -u origin main` 将本地仓库push到远程仓库(*main分支*)。

> 当对工作区修改（或新增）的文件执行 **git add** 命令时，暂存区的目录树被更新，同时工作区修改（或新增）的文件内容被写入到对象库中的一个新的对象中，而该对象的ID被记录在暂存区的文件索引中。
>
> 当执行提交操作（git commit）时，暂存区的目录树写到版本库（对象库）中，master 分支会做相应的更新。即 master 指向的目录树就是提交时暂存区的目录树。
>
> 

