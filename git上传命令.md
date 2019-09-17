# 将本地代码上传到github
### 在github中创建代码仓库，这个仓库中几乎是空白，本地工程中有完整的需要提交的代码，通过git init、git remote add、git push等命令来完成。

### 执行git add .，将本地的工程目录（包括子文件）都添加到本地的git仓库

### 执行git commit -m "write some comment"，将本地的工程提交到本地的git仓库

### 执行git remote add origin [github_repository_url]，将本地仓库与github上的仓库关联起来。
可以通过git remote -v查看github上的仓库地址。

### 执行git pull origin master同步github仓库和本地仓库

### 执行git push origin master将本地工程提交到github
## git设置用户名密码
~~~
git config --global user.name [username]
git config --global user.email [email]

~~~
## fatal: remote origin already exists.
### 先删除远程 Git 仓库
~~~
$ git remote rm origin
~~~
### 再使用 
~~~
git remote add origin [github_repository_url]
~~~