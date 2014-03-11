#Data-Scientis#
##一、LInux开发环境配置##
###1.1、开发工具介绍###
- [R](http://www.r-project.org/ "R")
- [Rstudio](https://www.rstudio.com/ "rstudio")
- [Git](http://git-scm.com/docs "Git")
- [jekyll](http://jekyllrb.com/ "jekyll")
- [latex](http://www.latex-project.org/ "latex")
- [Ruby](https://www.ruby-lang.org/zh_cn/ "Ruby")
- [rubygems](http://rubygems.org/ "rubygems")  

###1.2、安装Linux操作系统###
     CentOS6.5_64bit  
###1.3、安装Ruby环境###
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
     
###1.4、Git常用方法###
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

###1.5、安装R环境###
     rpm -Uvh http://mirror01.idc.hinet.net/EPEL/6/i386/epel-release-6-7.noarch.rpm  下载库
     yum search r-project 搜索R
     yum install R.x86_64 R-devel.x86_64 R-java.x86_64 安装R
     下载rstudio-0.98.501-x86_64.rpm IDE rpm
     rpm -ivh rstudio-0.98.501-x86_64.rpm 安装IDE

     
##二、Windows开发环境配置##
	python2.7
	ruby
	R
	rstuio
	jekyll
	
##三、安装注意事项##
      1. Rmd文件(通过脚本)KnitPost.R生成md文件，默认在根目录，无法自动到_post文件下
      2. 关于pygments高亮的问题							
      3. pygments版本问题	pygments 0.5.0/0.5.4才行，建议用Gemfile, 然后bundle install, bundle exec jekyll          serve来运行						
      4. css位置	生成的css在我的环境下只能放项目根目录下才起作用 pygmentize -S default -f html > pygments.css
       <head>						
	  <link rel="stylesheet" href="/pygments.css">					
      5. {% highlight language %} 和 {% endhighlight %}	r高亮不能，需要改为s才行				
       建议rstudio写rmd还是用```{r}，生成的md文件改为s就好了。Latex代码不会自动改```为%highlight%，这个也要手动添加						
								
      6 关于Rstudio——>jekyll的过程							
      7.Rstudio打开Rproj						
      8.source("_posts/KnitPost.R")						
      9.KnitPost("_drafts/2014-03-03-RmdTest.Rmd")						
      10.将根目录下的2014-03-03-RmdTest.md拷贝到_post文件夹（注意如果用rstudio编译预览过，_draft下会生成html，md，                figure，不要理会。_draft下保存rmd文件，其余可删）	   
      11.修改2014-03-03-RmdTest.md中的highlight部分						
      12.bundle exec jekyll serve						

