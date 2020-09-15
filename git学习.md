## Git是什么？
[TOC]
来自<a href="https://www.liaoxuefeng.com/wiki/896043488029600">廖雪峰git教程</a>
> Git是目前世界上最先进的分布式版本控制系统（没有之一）

CVS,SVN都是版本控制系统，集中式的，需要联网使用。

#### 集中式？分布式？
> 集中式版本控制系统，版本库是集中存放在中央服务器的，而干活的时候，用的都是自己的电脑，所以要先从中央服务器取得最新的版本，然后开始干活，干完活了，再把自己的活推送给中央服务器。中央服务器就好比是一个图书馆，你要改一本书，必须先从图书馆借出来，然后回到家自己改，改完了，再放回图书馆。

<b>总结：</b>中央服务器是必须的，要通过中央服务器实现代码修改。

> 分布式版本控制系统根本没有“中央服务器”，每个人的电脑上都是一个完整的版本库，这样，你工作的时候，就不需要联网了，因为版本库就在你自己的电脑上。

<b>总结：</b>伪“中央服务器”只实现代码修改的交换。

#### git的安装和仓库的建立

* mac系统
1. homebrew <a href="http://brew.sh/">具体参考homebrew开发文档</a>
2. 下载xcode 现在xode对我来说有点难用

* 创建版本库（仓库：repository）
1. 新建空文件夹用来存放git项目

``` 
$ mkdir learngit
$ cd learngit
$ pwd
/Users/xiexiaomeng/learngit

```
创建一个空文件夹，目录为` /Users/xiexiaomeng/learngit`

2.  通过git init命令把这个目录变成Git可以管理的仓库

```
$ git init
```

3. 在git项目文件夹中创建或·修改文件
* add
`  git add <file>`

* commit
`  git commit -m <message>`


> commit 可以用来添加多个文件

<b>例子：</b>
```
$ git add file1.txt
$ git add file2.txt file3.txt
$ git commit -m "add 3 files."
```

#### git   版本的修改，回退，再回退
   * ` head`指向的版本就是当前版本 使用命令` git reset --hard commit_id` 可以回到过去
   *  ` git log`可以查看提交历史，找到版本号` commit_id`
   *  ` git reflog`查看命令历史，确定未来找到哪个版本号

#### git的暂存区和工作区
   * 工作区 版本库（暂存区（stage） master）
   * ` add`操作将工作区文件添加到暂存区
   * ` commit`操作将暂存区一次性提交到master
   * ` get status`可以看工作区状态（文件是否有被修改，是否添加到缓存区）

#### git追踪修改
    如果不add第二次修改，将无法commit；
    可以同时commit两次修改
    

#### 撤销修改
 可以通过` git status`看如何撤销
   * 场景1:丢弃工作区的修改：` git checked --file`
   * 场景2:撤销添加到暂存区：` git reset HEAD <file>`,再执行第一步
   * 场景3:已提交至版本库，参见版本回退。

#### 文件删除
 ` git rm`用于删除一个文件
  如果一个文件已经被提交到版本库，那么你永远不用担心误删(使用` git checkout --file`撤销删除)，但是要小心，你只能恢复文件到最新版本，你<b>会丢失最近一次提交后你修改的内容</b>


### git的远程仓库
#### 添加远程库
 1. 关联一个远程库，使用命令 ` git remote add origin git@server-name:path/repo-name.git`;
 2. ` git push -u origin master`第一次推送(所有内容)
 3. ` git push origin master` 推送最新修改
 有网络的时候完成同步

#### 从远程库克隆
 1. 新建仓库
 2. 本地新建文件夹
 2. ` git clone 仓库地址` 可以使用ssh也可以使用https

### 分支管理
1. 





