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
     
###2.4、Git常用方法###
     // 先checkout master （如果没做过这一步）
     git clone <git-repos-url> (如<git@...>或者<https://...>)

     // checkout branch：
     git checkout <branch-name>
     git add <dir> or <files>  （如有新增目录或文件）
     git ci -a
     （弹出vi，写comment，wq退出）
     git push

     // 合并 
     git checkout <master-name>
     git branches  （查看有哪些branch）
     git merge <branch-name>

###2.5、安装R环境###
     rpm -Uvh http://mirror01.idc.hinet.net/EPEL/6/i386/epel-release-6-7.noarch.rpm  下载库
     yum search r-project 搜索R
     yum install R.x86_64 R-devel.x86_64 R-java.x86_64 安装R
     下载rstudio-0.98.501-x86_64.rpm IDE rpm
     rpm -ivh rstudio-0.98.501-x86_64.rpm 安装IDE
##三、项目开发流程##
##四、项目参与方法##
