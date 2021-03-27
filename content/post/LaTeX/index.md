---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "LaTeX"
subtitle: ""
summary: "LaTeX（音译“拉泰赫”）是一种基于ΤΕΧ的排版系统"
authors: []
tags: []
categories: []
date: 2020-04-27T16:12:48+08:00
lastmod: 2020-04-27T16:12:48+08:00
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
- LaTeX（音译“拉泰赫”）是一种基于ΤΕΧ的排版系统，由美国计算机学家莱斯利·兰伯特（Leslie Lamport）在20世纪80年代初期开发。
利用这种格式，即使使用者没有排版和程序设计的知识也可以充分发挥由TeX所提供的强大功能，能在几天，甚至几小时内生成很多具有书籍质量的印刷品。
- 对于生成复杂表格和数学公式，这一点表现得尤为突出。因此它非常适用于生成高印刷质量的科技和数学类文档。这个系统同样适用于生成从简单的信件到完整书籍的所有其他种类的文档。

## Install

从[清华镜像源](https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/Images/)下载对应操作系统的Texlive软件包
```sh
# 安装
sudo ./install-tl   
# 设置环境变量
# LaTeX
export TEX_HOME=/usr/local/texlive/2019
export PATH=$PATH:$TEX_HOME/bin/x86_64-linux
export INFOPATH=$INFOPATH:$TEX_HOME/texmf-dist/doc/info
export MANPATH=$MANPATH:$TEX_HOME/texmf-dist/doc/man
```            

## 安装 Windows 字体
```sh
# 创建 win 下字体专用文件夹
sudo mkdir /usr/share/fonts/winfonts

# 复制windows上的字体到/usr
sudo cp your_winfonts_dir /usr/share/fonts/winfonts 

# 进入字体文件夹
cd /usr/share/fonts/winfonts

# 修改访问权限
sudo chmod 744 *

# 回到主目录
cd ~

# 更新字体信息
sudo mkfontscale
sudo mkfontdir
sudo fc-cache -f -v
```

## More
[LaTeX模板](http://github.com/Lucas-Wye/Latex_template)  
[LaTeX开源小屋](http://latexstudio.net/)  
[LaTeX Introduction](https://github.com/Lucas-Wye/Share/tree/master/LaTeX)  
[TeX Live下载及安装说明](https://liam.page/texlive/)  
[一份其实很短的 LaTeX 入门文档](https://liam.page/2014/09/08/latex-introduction/)
