# GIT Learing
## Git是一个分布式的版本管理系统。

* 分布式是指所有的git服务器的地位都是相等没有主次之分
* 版本管理是指在存储每次修改的代码的不同版本并附上版本号，这样就可以在出错了的时候，方便地返回旧版本。

## Git常用的命令

* git -h 是git帮助命令
* git init 是在git服务器上创建git代码库
* git status 显示当代代码仓库的状态。
* git commit -m "xxx" 是改修改的文件检入代码仓库，并提供"xxx"的附加信息。
* git log 是查看存储了的版本以及信息
* git branch -M main 是更改分支名字为main。
* git add 是讲文件加入stage区
* git add .  可以添加目录里所有的文件
* git remote add 远程服务器名称 远程URL 将本地服务器和远程服务器相关联。
* git push origin main -u 是将已经修改的文件push到远程服务器。第二次将不需要使用-u
* git pull origin main 将远程服务器的代码库的内容拉到本地服务器。
* git remote add origin https://<用户名>:<密码>@远程URL   关联远程服务器第二种方法。
* git remote rm origin 删除关联的远程服务器。
* git remote set-url origin 修改关联的远程服务器。
* git remote update --prune 将远程的信息同步到本地服务器，但不改变本地代码
* git fetch origin 也是将远程的信息同步到本地服务器，也不改变本地代码，和update的区别是一次性只同步一个remote或者branch的信息。
* git remote -v 看git关联的信息

### .gitignore
* .gitignore文件是忽略指定的文件或文件夹。

* 这些指定的文件或者文件夹是不能push到github。
  * 比如系统自动生成的文件，不一定能够兼容，有可能使用的操作系统不一样。
  * 比如存储个人私密信息的文件，push会泄露自己的信息，出现不必要的安全隐患。
* .gitignore文件里指定这些文件名或者文件夹的路径，那么git就会忽略这些文件或文件夹。不会在untracked files表里一直提示你要添加这些文件，以免出现错误的操作push到github中。
* ***注：如果不commit .gitignore文件，将无法得知这个项目忽略那些文件或者文件夹，其他程序员为这个项目添加新功能，会不知道忽略什么文件或者文件夹，有可能会push忽略的文件或者文件夹***

### bash常用命令

* touch 是创建新文件
* mv 移动文件
* cp 拷贝文件
* rm 删除文件
* rm -rf 删除文件夹
* mkdir 创建文件夹
* ls -al 列出包含隐藏文件夹在内的文件

      
