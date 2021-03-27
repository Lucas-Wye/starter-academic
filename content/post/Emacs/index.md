---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Emacs"
subtitle: ""
summary: "GNU Emacs, An extensible, customizable, free/libre text editor — and more."
authors: []
tags: []
categories: []
date: 2021-01-22T09:56:53+08:00
lastmod: 2021-01-22T09:56:53+08:00
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
- GNU Emacs, An extensible, customizable, free/libre text editor — and more. 
- At its core is an interpreter for Emacs Lisp, a dialect of the Lisp programming language with extensions to support text editing.

## Cursor movement
|      |          |
| ---- | -------- |
| C-v | Move forward one screenful |
| M-v | Move backward one screenful |
| C-l | Clear screen and redisplay all the text |
| C-n | Move next line |
| C-p | Move previous line |
| C-f | Move forward a character |
| C-b | Move backward a character |
| M-f | Move forward a word |
| M-b | Move backward a word |
| C-a | Move to beginning of line |
| C-e | Move to end of line |
| M-a | Move back to beginning of sentence |
| M-e | Move forward to end of sentence |
| M-< | Move to the beginning of file |
| M-> | Move to the end of file |
| C-u NUM | (Prefix) repeat NUM times |
| C-g | stop/cancel current execution |


## Insert and Delete
|      |          |
| ---- | -------- |
| DEL | delete the character just before the cursor |
| C-d | delete the next character after the cursor |
| M-DEL | kill the word immediately before the cursor |
| M-d | kill the next word after the cursor |
| C-k | kill from the cursor position to end of line |
| M-k | kill to the end of the current sentence |
| C-SPACE + [Move Cursor] | select text |
| C-y | yank the more recent killed text back |
| M-y | replace the yanked text with the previous kill |
| C-/, C-_, C-x u | Undo |


## File and Buffer
|      |          |
| ---- | -------- |
| C-x C-f | find a file |
| C-x C-s | save the file |
| C-x C-b | list buffers |
| C-x b | switch buffer |
| C-x s | save some buffers |
| C-x C-c | quit the Emacs session |
| C-z | exit Emacs temporarily |
| M-x | prefix of some commands |


## Search 
|      |          |
| ---- | -------- |
| C-s | search forward |
| C-r | search backward |


## Windows
|      |          |
| ---- | -------- |
| C-x 1 | get rid of extra windows and go back to basic one-window editing |
| C-u 0 C-l | 
| C-h k C-f | 
| C-x 2 | split the screen into two windows |
| C-M-v | scroll the bottom window | 
| C-v o | move the cursor to the other window |


## More

