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

### Git特殊的文件

* 由于我们在搭建依赖环境或者在编译的时候，总会有一些系统自己生成的文件别的系统不一定能用或者是我们存储的密码配置等一般不push 到GitHUB，
但是当git commit的时候会一直显示在Untrached files，我们为了让git不要在显示这些信息。我们可以创建.gitkeep的文件并打开文件在里面填写
要忽略的文件名就可以让git这些文件。

### bash常用命令

* touch 是创建新文件
* mv 移动文件
* cp 拷贝文件
* rm 删除文件
* rm -rf 删除文件夹
* mkdir 创建文件夹
* ls -al 列出包含隐藏文件夹在内的文件

      
