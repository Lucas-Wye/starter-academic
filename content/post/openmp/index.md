---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "OpenMP"
subtitle: ""
summary: "OpenMP是由OpenMP Architecture Review Board牵头提出的，并已被广泛接受的，用于共享内存并行系统的多线程程序设计的一套编译指令 (Compiler Directive)"
authors: []
tags: []
categories: []
date: 2019-10-04T15:03:25+08:00
lastmod: 2020-04-27T15:03:25+08:00
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
- OpenMP是由OpenMP Architecture Review Board牵头提出的，并已被广泛接受的，用于共享内存并行系统的多线程程序设计的一套编译指令 (Compiler Directive)。

## Introduction
See detail at [wiki](https://en.wikipedia.org/wiki/OpenMP).

## OpenMP Programming Example
Here is a C program using OpenMP.
```C
#include<stdio.h>
#include<omp.h>

int main(void) {
    const int n = 10;
    int arr[n];

    #pragma omp parallel for  
    for(int i = 0;i < n;i++) {
        arr[i] = i;
        printf("%d\n",i);
    }

    for(int j = 0;j < n;j++){
        printf("%d\n",arr[j]);
    }

    return 0;      
}
```

## More Example
[OpenMP并行开发（C++） ](https://zhuanlan.zhihu.com/p/51173703)  
[OpenMP并行程序设计（二）](https://blog.csdn.net/drzhouweiming/article/details/1175848)
