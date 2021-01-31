---
layout: post
title:  "Github Page with Jekyll!"
date:   2021-01-22 13:15:44 +0800
categories: Github Page
---
## What is Jekyll
Jekyll 是一个简单的 适于创作blog的 静态网站生成工具，github发起人Tom用ruby语言写的，使用MIT许可。

## Install
```sh
# install ruby
brew install ruby # 安装了ruby 3.0.0
```
```sh
# vim ~/.bash_profile 添加下列内容
# Ruby Setup
#export DLN_LIBRARY_PATH=~/.myruby/lib
export LOGDIR=~/.myruby/log
export LOGNAME=aren
export RUBYROOT=/usr/local/Cellar/ruby/3.0.0_1
export RUBYPATH=$RUBYROOT/bin
export RUBYLIB=$RUBYROOT/lib
#export RUBY_PREFIX=
#export RUBYOPT=
#export RUBYSHELL=
export PATH=$RUBYPATH:$PATH
# Gem Setup
export GEM_ROOT=/usr/local/lib/ruby/gems/3.0.0
export GEM_HOME=$GEM_ROOT/gems
export GEM_PATH=$GEM_ROOT
export PATH=$GEM_PATH/bin:$PATH
```
```sh
# install jekyll & take a shoot
mkdir -p work/ruby
cd work/ruby
gem install jekyll bundler
gem install rexml
jekyll new mysite

cd mysite
bundle install
bundle add webrick
bundle exec jekyll serve
```
然后就可以通过访问最后一个命令输出在终端的地址，访问网站了。

## Post
这篇Post原是Jekyll的示例，位于`_posts`目录，经过重新编辑，重建而来。
通常使用`jekyll serve`重新启动服务、重建网站。

Jekyll Post格式:`YEAR-MONTH-DAY-title.MARKUP`


Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
