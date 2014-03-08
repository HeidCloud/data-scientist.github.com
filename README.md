#Data-Scientist 项目引导#

##一、项目简介##
     待写
##二、项目环境配置##
###2.1、开发工具介绍###
- [R](http://www.r-project.org/ "R")
- [Rstudio](https://www.rstudio.com/ "rstudio")
- [Git](http://git-scm.com/docs "Git")
- [jekyll](http://jekyllrb.com/ "jekyll")
- [latex](http://www.latex-project.org/ "latex")
- [Ruby](https://www.ruby-lang.org/zh_cn/ "Ruby")
- [rubygems](http://rubygems.org/ "rubygems")  
###2.2、安装Linux操作系统###  
     CentOS6.5_64bit  
###2.3、安装Ruby环境###  
     1、安装系统相关依赖包  
     yum install gcc-c++ patch readline readline-devel zlib zlib-devel 
     yum install libyaml-devel libffi-devel openssl-devel make 
     yum install bzip2 autoconf automake libtool bison iconv-devel
     2、安装RVM(Ruby版本管理器-Ruby Version Manager)
     curl -L get.rvm.io | bash -s stable
     3、设置RVM环境
     source /etc/profile.d/rvm.sh
     4、安装1.9.3版本Ruby
     rvm install 1.9.3
     5、查看Ruby版本
     ruby --version
     6、安装Ruby Gems
     yum install rubygems
     7、安装Ruby bundler
     gem install bundler
     8、安装jekyll
     gem install jekyll
     9、安装git
     yum install git
     10、下载项目
     git clone https://github.com/Data-Scientist/data-scientist.github.com.git
     11、运行项目
     jekyll serve
     12、本地访问项目
     http://youIp:4000(访问前最好关闭防火墙)     
###2.4、安装jekyll###  
###2.5、Git常用方法###  
##三、项目开发流程##  
##四、项目参与方法##  
