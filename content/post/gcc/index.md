---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "GCC"
subtitle: ""
summary: "GCC编译器也称为Linux GCC命令，它有很多选项。GCC编译器是Linux下最常用的编译器"
authors: []
tags: []
categories: []
date: 2019-10-16T15:57:07+08:00
lastmod: 2020-04-27T15:57:07+08:00
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
- GCC编译器也称为Linux GCC命令，它有很多选项。GCC编译器是Linux下最常用的编译器。

## Install
```sh
# MacOS安装Xcode工具链                                
xcode-select --install
# Ubuntu
sudo apt install gcc
```

## Basic
```sh
gcc -c filename.c # compile only, produce .o
gcc -g # compile for debugging
gcc -o filename.o # 
gcc -O 1,2,3,4,s,fast # for optimization level
gcc -Ipathname
gcc -Dsymbol # define preprocessor symbol
gcc -Ldirectory # add directory to the library search path
gcc -lxyz # link with library libxyz.a or libxyz.so
```

## gdb
```sh
gdb BINARY_FILE
list
br 8 # breakpoint in line 8
run
print value 
next
where
help
quit
```

## make
(1)Predefined Macros  
- AS - assembler (as)
- CC - C compiler command (cc)
- FC - Fortran compiler command (fc)
- CPP - C++ preprocessing command ($(CC) -E)
- CXX - C++ compiler command (g++)
- CFLAGS - C compiler option flags (e.g. -g)
- FFLAGS - Fortran compiler option flags (e.g. -g)
- LDFLAGS - Linking option flags (e.g. –L /usr/share/lib)
- LDLIBS – Linking libraries (e.g. -lm)  

(2)Special Internal Macros
```sh
$* # The basename of the current target
$< # The name of a dependency file, as we see on last page
$@ # The name of the current target.
$? # The list of dependencies that are newer than the target.
```

## More
[more of gdb](https://blog.csdn.net/gatieme/article/details/51671430)  
[Makefile example](https://github.com/Lucas-Wye/Makefile-Templates)