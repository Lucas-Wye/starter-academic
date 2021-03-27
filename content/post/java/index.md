---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Java"
subtitle: ""
summary: "Java 是由Sun Microsystems公司于1995年5月推出的高级程序设计语言"
authors: []
tags: []
categories: []
date: 2020-04-27T15:59:14+08:00
lastmod: 2020-04-27T15:59:14+08:00
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
- Java 是由Sun Microsystems公司于1995年5月推出的高级程序设计语言。 Java可运行于多个平台，如Windows, Mac OS，及其他多种UNIX版本的系统。

## Install
[JDK](https://www.oracle.com/technetwork/java/javase/downloads/index.html)  
[IntelliJ IDEA](https://www.jetbrains.com/idea/)
```sh
# 配置环境变量                                
export JAVA_HOME=/usr/lib/jvm/jdk1.8.0_144  # 这里换成自己的jdk目录
export JRE_HOME=${JAVA_HOME}/jre  
export CLASSPATH=.:${JAVA_HOME}/lib:${JRE_HOME}/lib  
export PATH=${JAVA_HOME}/bin:$PATH
```

## Usage of adb(Android Debug)
```sh
# 卸载系统软件
adb shell
pm list package
pm uninstall -k --user 0 package_name
```
