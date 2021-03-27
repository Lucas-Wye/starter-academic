---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Kali"
subtitle: ""
summary: "Kali Linux是基于Debian的Linux发行版， 设计用于数字取证操作系统"
authors: []
tags: []
categories: []
date: 2019-10-16T16:02:51+08:00
lastmod: 2020-04-27T16:02:51+08:00
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
- Kali Linux是基于Debian的Linux发行版， 设计用于数字取证操作系统。由Offensive Security Ltd维护和资助。最先由Offensive Security的Mati Aharoni和Devon Kearns通过重写BackTrack来完成，BackTrack是他们之前写的用于取证的Linux发行版。
- Kali Linux预装了许多渗透测试软件，包括nmap 、Wireshark 、John the Ripper，以及Aircrack-ng；用户可通过硬盘、live CD或live USB运行Kali Linux。Kali Linux既有32位和64位的镜像。可用于x86 指令集。同时还有基于ARM架构的镜像，可用于树莓派和三星的ARM Chromebook。


## Install
```sh
# 从Docker安装
docker pull kalilinux/kali-linux-docker
# 运行
docker run -t -i kalilinux/kali-linux-docker /bin/bash
```

## More
[kali官网](https://www.kali.org/)
