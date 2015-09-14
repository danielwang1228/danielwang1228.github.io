---
layout: post
category : lessons
tagline: "Supporting tagline"
tags : [intro, beginner, jekyll, tutorial]
---
{% include JB/setup %}

最近发现Github + jekyee用来写博客确实方便，可以更专注内容，唯一的缺点就是配置上有点点麻烦，这里做个笔记以备用。

## 前提
Windows 7系统；已经安装了git工具；有一个github的帐号。

## 开始安装：

### 安装ruby
安装rubyinstaller-2.x.x-xxx.exe，确保在某个目录下(不能有中文和空格)，如：D:/ruby2
配置PATH环境变量。(安装时可选择自动配置)。

### 安装DevKit

#### 释放文件
释放DevKit-mingw64-xx-xxx-sfx.exe 到某个目录(不能有空格和中文)。

#### 增强Ruby:

    cd “xxx\DevKit”
    ruby dk.rb init
    ruby dk.rb install

### 安装Jekyll

####　更改源
    gem sources --remove https://rubygems.org/
    gem sources -a https://ruby.taobao.org/
    gem sources -l         #查看是否只有taobao镜像
    gem update --system    #更新RubyGems软件


#### 安装jekyll
    gem install jekyll 

### 安装Python 2.7

#### 安装easy_install(ez_setup)

    python distribute_setup.py
    
#### 安装Pygments 

    easy_install Pygments
    
### 测试
    jekyll new myblog
    cd myblog
    jekyll serve

打开浏览器输入：http://127.0.0.1:4000

## 使用github page

#### 新建仓库

登录github，新建名为 username.github.io 的仓库
克隆仓库到本地。

    git clone xxxx


#### 安装Jekyll-Bootstrap

    git clone https://github.com/plusjade/jekyll-bootstrap.git

复制里面除了.git以外的目录，到username.github.io工作区目录。启动jekyll

    jekyll serve
    
### 打开浏览器输入：http://127.0.0.1:4000
