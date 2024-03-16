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

> git add 并不是"添加文件"，而是类似添加更改，如果add一个文件，再进行commit，那么add的文件会和本地仓库进行比较，有更改的才会被add，之后才commit

