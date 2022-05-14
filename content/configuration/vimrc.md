---
title: "vimrc configuration"
date: 2022-05-14
menu: "configuration"
weight: 1
---

Place this file globally in /etc/vim/vimrc or ~/.vimrc


```
"Use vim settings, rather then vi settings
set nocompatible

"Syntax highlighting
syntax on

"Disable mouse settings for Vim and leave this to the terminal gui
set mouse=
set ttymouse=

"Show on the left the line number
set number

"Show the line and column number of the cursor position"
set ruler

"Highlight currentline
set cursorline

"A tab is four spaces
set tabstop=2
"A tab is four spaces
set softtabstop=2

"Always show the statusbar
set laststatus=2

"Show a redline at charater position 81
set cc=81

"Highlight search terms
set hlsearch

"Show search matches as you type
set incsearch

"Do not show hidden characters
set nolist

"Bonus, uncomment this feature!
"Create backup files in ~/tmp. Directory needs to exist

"set backup
"let bac_var = strftime(".%y-%m-%d-%H-%M")
"set backupdir=~/tmp/
"let bac_var = "set backupext=" . bac_var
"execute bac_var
```
