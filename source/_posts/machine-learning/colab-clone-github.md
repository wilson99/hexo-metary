---
title: colab clone github至google drive
top: false
cover: true
toc: true
mathjax: true
date: 2020-11-19
password:
summary:
tags: colab
categories: Machine Learninig
---


``` python
from google.colab import drive
drive.mount('/content/drive')

%cd '/content/drive/MyDrive'

import os
!mkdir researchHub
os.chdir('./researchHub/')

!git clone --depth=1 https://github.com/ageron/handson-ml2
os.chdir('./handson-ml2')
!pwd
```
