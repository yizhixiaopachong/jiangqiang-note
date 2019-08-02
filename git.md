### git 简单使用

Git 是 Linux 发明者 Linus 开发的一款新时代的版本控制系统，那什么是版本控制系统呢？怎么理解？

我们在软件开发中源代码其实是最重要的，那么对源代码的管理变得异常重要：

比如为了防止代码的丢失，肯定本地机器与远程服务器都要存放一份，而且还需要有一套机制让本地可以跟远程同步；

又比如我们经常是好几个人做同一个项目，都要对一份代码做更改，这个时候需要大家互不影响，又需要各自可以同步别人的代码；

又比如我们开发的时候免不了有 bug，有时候刚发布的功能就出现了严重的 bug，这个时候需要紧急对代码进行还原；
又比如随着我们版本迭代的功能越来越多，但是我们需要清楚的知道历史每一个版本的代码更改记录，甚至知道每个人历史提交代码的情况；

等等等类似以上的情况，这些都是版本控制系统能解决的问题。所以说，版本控制是一种记录一个或若干文件内容变化，以便将来查阅特定版本修订情况的系统，对于软件开发领域来说版本控制是最重要的一环，而 Git 毫无疑问是当下最流行、最好用的版本控制系统。

### 下载安装

-   git 官网 下载
-   安装即可

### git 的四个区域

-   工作区 (操作代码)
-   暂存区 add
-   本地仓库 commit
-   远程仓库 push
    ![git](https://user-gold-cdn.xitu.io/2019/1/23/168766ec478de231?imageView2/0/w/1280/h/960/format/webp/ignore-error/1)

### git 配置

-   配置信息列表
    git config --list

-   设置用户名
    git config --global user.name "John Doe"

-   设置邮箱
    git config --global user.email johndoe@example.com

### 简单命令

-   git init 初始化本地仓库
-   git status 查看文件状态 (红色就是没有添加到暂存区,绿色就是已经添加到了暂存区,绿色红色都没有(目前工作区文件都已提交到了本地仓库))
-   git add 文件名 (将文件添加到 暂存区)
-   git add . (将所有文件添加到 暂存区)
-   git commit -m'提交信息' 暂存区内容 提交到本地仓库
-   git remote add origin [url]
-   git push origin master

### 如何上传笔记到 github 仓库

-   右键 git bash here 黑窗口
-   git init
-   git add .
-   git commit -m''
-   git git remote add origin [url](只需第一次)
-   git push origin master
