---
layout: post
title: "JekyllBootstrap简介"
description: "简单的静态web"
category: web
tags: [jekyll]
---
{% include JB/setup %}

安装
----
在github上建立一个名为USERNAME.github.com的仓库，*USERNAME*是你的用户名

	$ git clone https://github.com/plusjade/jekyll-bootstrap.git USERNAME.github.com
	$ cd USERNAME.github.com
	$ git remote set-url origin git@github.com:USERNAME/USERNAME.github.com.git
	$ git push origin master
    
在本地运行

	$ gem install jekyll
    $ cd USERNAME.github.com
    $ jekyll serve
    
post
-----

	$ rake post title="Hello World"
    
    $ rake page name="about.md"
    $ rake page name="pages/about.md"
    $ rake page name="pages/about"
    
上传到github

	$ git add .
	$ git commit -m "Add new content"
	$ git push origin master
    