---
title: VIM Plugins
top: false
cover: true
toc: true
mathjax: true
date: 2021-1-4
password:
summary:
tags: Linux
categories: Linux
---

### VundleVIM
[VundleVim/Vundle.vim: Vundle, the plug-in manager for Vim (github.com)](https://github.com/VundleVim/Vundle.vim)

#### 1. git clone
```
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
#### 2. vi ~/.vimrc
```
set nocompatible " be iMproved, required
filetype off " required

" set the runtime path to include Vundle and initialize
set rtp+=~/.vim/bundle/Vundle.vim
call vundle#begin()
" alternatively, pass a path where Vundle should install plugins
"call vundle#begin('~/some/path/here')

" let Vundle manage Vundle, required
Plugin 'VundleVim/Vundle.vim'

" The following are examples of different formats supported.
" Keep Plugin commands between vundle#begin/end.
" plugin on GitHub repo
Plugin 'tpope/vim-fugitive'
" plugin from http://vim-scripts.org/vim/scripts.html
" Plugin 'L9'
" Git plugin not hosted on GitHub
Plugin 'git://git.wincent.com/command-t.git'
" git repos on your local machine (i.e. when working on your own plugin)
Plugin 'file:///home/gmarik/path/to/plugin'
" The sparkup vim script is in a subdirectory of this repo called vim.
" Pass the path to set the runtimepath properly.
Plugin 'rstacruz/sparkup', {'rtp': 'vim/'}
" Install L9 and avoid a Naming conflict if you've already installed a
" different version somewhere else.
" Plugin 'ascenator/L9', {'name': 'newL9'}

" All of your Plugins must be added before the following line
call vundle#end() " required
filetype plugin indent on " required
" To ignore plugin indent changes, instead use:
"filetype plugin on
"
" Brief help
" :PluginList       - lists configured plugins
" :PluginInstall    - installs plugins; append \`!\` to update or just :PluginUpdate
" :PluginSearch foo - searches for foo; append \`!\` to refresh local cache
" :PluginClean      - confirms removal of unused plugins; append \`!\` to auto-approve removal
"
" see :h vundle for more details or wiki for FAQ
" Put your non-Plugin stuff after this line
```
#### 3. vim +PluginInstall +qall

### YouCompleteMe
[ycm-core/YouCompleteMe: A code-completion engine for Vim (github.com)](https://github.com/ycm-core/YouCompleteMe)
#### 1. Add into ~/.vimrc
```
Plugin 'ycm-core/YouCompleteMe'
```
#### 2. :PluginInstall
#### 3. Compile
```
cd ~/.vim/bundle/YouCompleteMe
python3 install.py --all
```
#### 4. Add into end of ~/.vimrc 
```
let g:ycm_global_ycm_extra_conf='~/.ycm_extra_conf.py'
```
#### optional. Add into ~/.ycm_extra_conf.py
```
'-isystem',
'/usr/local/include/opencv4',
```

[preservim/nerdtree: A tree explorer plugin for vim. (github.com)](https://github.com/preservim/nerdtree)

[Raimondi/delimitMate: Vim plugin, provides insert mode auto-completion for quotes, parens, brackets, etc. (github.com)](https://github.com/Raimondi/delimitMate)

