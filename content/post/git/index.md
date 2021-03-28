---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Git"
subtitle: ""
summary: "Git 是一个开源的分布式版本控制系统，用于敏捷高效地处理任何或小或大的项目"
authors: []
tags: []
categories: []
date: 2019-10-16T15:30:21+08:00
lastmod: 2020-04-27T15:30:21+08:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
- Git 是一个开源的分布式版本控制系统，用于敏捷高效地处理任何或小或大的项目。
- Git 是 Linus Torvalds 为了帮助管理 Linux 内核开发而开发的一个开放源码的版本控制软件。
- Git 与常用的版本控制工具 CVS, Subversion 等不同，它采用了分布式版本库的方式，不必服务器端软件支持。

### 创建版本库
```sh
git init
git clone URL
```

### 修改和提交
```sh
git status
git diff FILE_NAME
git add FILE_NAME
git mv OLD_NMAE NEW_NAME
git rm FILE_NAME
git rm --cached FILE_NAME # 停止跟踪文件但不删除
git commit -m YOUR_COMMENT
git commit --amend
```

### 查看提交历史
```sh
git log
git reflog # 所有分支信息
git log -p FILE_NAME # 查看指定文件的提交历史
git blame FILE_NAME # 以列表方式查看指定文件的提交历史
```

### 撤销
```sh
git reset HEAD
git reset --hard HEAD
git checkout HEAD FILE_NAME
git revert COMMIT_ID
```

### 分支与标签
```sh
git branch
git checkout BRANCH/TAG
git branch NEW_BRANCH
git branch -d BRANCH
git tag # 列出所有的本地标签
git tag TAG_NAME # 基于最新的提交创建标签
git tag -d TAG_NAME
```

### 合并与衍合
```sh
git merge BRANCH
git rebase BRANCH
```

### 远程操作
```sh
git remote -v
git remote show REMOTE # 查看指定远程版本库信息
git remote add REMOTE URL

git fetch REMOTE
git pull REMOTE BRANCH
git push REMOTE BRANCH
git push REMOTE:BRANCH:TAG
git push --tags
```

### 垃圾回收  
Git仓库越来越臃肿，大多数版本控制系统存储的是一组初始文件， 以及每个文件随着时间的演进而逐步积累起来的差异；  而Git则会把文件的每一个差异化版本都记录在案。
这意味着，即使你只改动了某个文件的一行内容， Git也会生成一个全新的对象来存储新的文件内容。

对象碎片：如果你改动了一个很大的文件， git会为这个文件生成了一个很大的Blob对象  
```sh
cd .git
du -ah  # 查看文件大小
git gc --prune=now # 垃圾回收
```
实际上，并不需要手动调用 gc 命令。每当碎片对象过多，或者你向远端服务器发起推送的时候，git 就会自动执行一次打包过程。

### submodule
```sh
# 添加子仓库
git submodule add <仓库地址> <本地路径>
# 检出子仓库
git submodule init # 初始化本地配置文件
git submodule update # 检出父仓库列出的commit 
## 或者
git submodule update --init --recursive
# 递归克隆
git clone <仓库地址> --recursive
```

### 合并多个commit
```
commit THIRD_COMMIT_ID
	add third commit

commit SECOND_COMMIT_ID
	add second_commit

commit FIRST_COMMIT_ID
	add third commit
```
首先有3个commit，需要将前两个commit合成一个
```sh
git rebase -i FIRST_COMMIT_ID
```
出现如下界面：
```sh
pick SECOND_COMMIT_ID add second_commit
pick THIRD_COMMIT_ID add third commit

...
```
修改成：
```sh
pick SECOND_COMMIT_ID add second_commit
squash THIRD_COMMIT_ID add third commit
```
DONE.

## More
[git教程](https://www.runoob.com/git/git-tutorial.html)  
