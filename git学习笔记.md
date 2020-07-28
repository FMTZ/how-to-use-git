参考B站git课程  https://www.bilibili.com/video/BV1iW411t7EN  做一个git操作的简单记录

1.创建仓库：git init fileName



2.基本使用

查看仓库状态：git status

将所有更改的文件添加到暂存区：git add .    添加某一文件：git add fileName

提交版本：git commit / git commit -m "..."

产看版本记录：git log 

返回到之前的某一个版本：git checkout 版本号前7位/或者更多位也可以

所以，在git中，任何一次修改都有如下过程：先做出一次修改，然后将更改添加到暂存区，最后提交版本。



3.三种状态

回到上一个状态：git checkout -

三种状态：文件已修改，已加入暂存区，已提交



4.标签

添加标签：git tag -a 标签 -m "描述信息"       默认的标签是添加到最近一个节点，如果想要添加到指定节点，需要添加相应版本号：git tag -a 标签 -m "描述信息" 版本

查看tag详细信息：git show 相应tag的名称



5.分支

没有分支前只有主线，为master。创建的分支可以自己命名。

创建分支：git branch 分支名称

切换到相应分支：git checkout 分支名称

2和3可以合并：git checkout -b 分支名       创建并且切换到分支



6.合并分支

eg：发现之前的代码有bug。

先回到某一节点：git checkout 节点号；

创建一个分支并切换到相应分支；

在相应分支上做处理；

返回之前分支：git checkout master（分支名称）

合并分支：git merge 分支名



7.远程仓库 （已github为例）

先在github上创建一个仓库，得到一个远程仓库地址

添加远程仓库：git remote add 远程名称（github） 远程地址

上传代码：git push -u 远程名称 分支名

拷贝仓库：git clone 仓库地址



8.如何多人远程合作

![image-20200728111918639](/Users/fmtz/Library/Application Support/typora-user-images/image-20200728111918639.png)









