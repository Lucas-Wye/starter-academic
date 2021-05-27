---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Rime"
subtitle: ""
summary: "RIME／中州韻輸入法引擎，是一個跨平臺的輸入法算法框架。"
authors: []
tags: []
categories: []
date: 2021-05-27T20:21:34+08:00
lastmod: 2021-05-27T20:21:34+08:00
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
- RIME／中州韻輸入法引擎，是一個跨平臺的輸入法算法框架。
- 基於這一框架，Rime 開發者與其他開源社區的參與者在 Windows、macOS、Linux、Android 等平臺上創造了不同的輸入法前端實現。

## [My configuration](https://github.com/Lucas-Wye/rc/tree/master/rime)
Ubuntu: ibus + ibus-rime
```sh
sudo apt install -y ibus-rime librime-data-double-pinyin
```
Android: [trime](https://github.com/osfans/trime)


## Windows配置[小鹤双拼](https://flypy.com/)
输入法设置->常规->添加方案，添加内容如下图
![](https://raw.githubusercontent.com/Lucas-Wye/rc/master/rime/Windows-Flypy.png)
