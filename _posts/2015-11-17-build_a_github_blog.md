---
title: 利用Github Pages搭建一个个人博客
layout: dq
date: 2015-11-17
categories: blog
tags: [Github]
description: 请阅读全部内容！
---
#前言

##为什么选择Github Pages?

Github Pages 有以下诸多优点：
1、github pages有300M免费空间，资料自己管理，保存可靠；

2、学着用 github，享受 github 的便利，上面有很多牛人，眼界会开阔很多；

3、顺便看看 github 工作原理，最好的团队协作流程；

4、github 是趋势；

5、就算 github 被墙了，还可以搬到国内的 gitcafe 中去。

![](http://cdnzz.ifanr.com/wp-content/uploads/2014/06/github.png)

##什么是Github Pages?

[Github Pages](http://pages.github.com/)是用来介绍你托管在Github上面的项目的，不过由于空间免费而且资源稳定，用来搭建自己的网站再好不过了。

#目录
0.0 [持续更新中](http://www.computereric.xyz/blog/build_a_github_blog/#updating)

1.0 [前言](http://www.computereric.xyz/blog/build_a_github_blog/#section)

1.0.1 [为什么选择 Github Pages?](http://www.computereric.xyz/blog/build_a_github_blog/#github-pages)

1.0.2 [什么是Github Pages?](http://www.computereric.xyz/blog/build_a_github_blog/#github-pages-1)

1.1 [目录](http://www.computereric.xyz/blog/build_a_github_blog/#section-1)

2.0 [注册Github](http://www.computereric.xyz/blog/build_a_github_blog/#github)

3.0 [新建仓库](http://www.computereric.xyz/blog/build_a_github_blog/#section-2)

3.0.1 [仓库个性化主题](http://www.computereric.xyz/blog/build_a_github_blog/#section-3)

4.0 [Jekyll详解](http://www.computereric.xyz/blog/build_a_github_blog/#jekyll)

4.0.1 [什么是Jekyll](http://www.computereric.xyz/blog/build_a_github_blog/#jekyll-2)

4.0.2 [博客必要文件](http://www.computereric.xyz/blog/build_a_github_blog/#section-5)

4.0.3 [博客自定义文件](http://www.computereric.xyz/blog/build_a_github_blog/#section-6)




#注册Github

首先，注册或者登录[Github](http://github.com/)。
![](http://www.computereric.xyz/cache/img/ghpages/1.png)

进去之后套餐选择<code>Free</code>就可以了，除非是有特殊需要，<code>Free</code>套餐基本上可以满足你的需求了。
![](http://www.computereric.xyz/cache/img/ghpages/2.png)

#新建仓库

接下来找到<code>Your Respositories</code>，你应该没有任何仓库，选择<code>+ New respositories</code>
![](http://www.computereric.xyz/cache/img/ghpages/3.png)

这时你需要注意的是，主仓库命名必须为<code>username.github.io</code>。其实<code>.io</code>换成<code>.com</code>也是可以的，但是不推荐。

至此为止，你的仓库算是建造完成了。你应该会看到这样的页面。
![](http://www.computereric.xyz/cache/img/ghpages/7.png)

##仓库个性化主题

登陆[Jekyll](http://jekyllthemes.org)，找到一个自己喜欢的主题，选择<code>Home</code>。在右上角找到<code>fork</code>，然后你在自己的仓库里就有了一个一模一样的仓库。不过你要做的就是把仓库的名称改为<code>username.github.io</code>，是不是非常简单呢！

#Jekyll详解

##什么是Jekyll

GitHub Pages为了提供对HTML内容的支持，选择了Jekyll作为模板系统，Jekyll是一个强大的静态模板系统，作为个人博客使用，基本上可以满足要求，也能保持管理的方便，你可以查看Jekyll官方文档。

你可以直接fork我的项目，然后改名，就有了你自己的满足Jekyll要求的文档了，当然你也可以按照下面的介绍自己创建。

##Jekyll基本结构

Jekyll的核心其实就是一个文本的转换引擎，用你最喜欢的标记语言写文档，可以是Markdown、Textile或者HTML等等，再通过layout将文档拼装起来，根据你设置的URL规则来展现，这些都是通过严格的配置文件来定义，最终的产出就是web页面。

##博客必要文件

<code>_config.yml</code>是该网页的配置文件，设置好了之后就不用理它了。

<code>includes</code>是用于存放一些小的可复用的模块，一般不用设置。

<code>_layouts</code>是用于存放该网页的模版文件的。

<code>_posts</code>是用来存放博客博文的，需要注意的是，这里面的文件名必须要<code>year-month-date-title.后缀</code>，例如这篇文章就是<code>2015-11-17-build_a_github_blog.md</code>，后缀可以选择<code>.md</code>，<code>.html</code>，或是<code>.textile</code>，这里推荐使用.md。

##博客自定义文件

<code>404.html</code>网址访问错误时弹出的错误信息。

<code>CNAME</code>用于绑定域名

其他文件或文件夹是可以随意创建的，例如我在<code>username.github.io</code>下创建了<code>project</code>文件夹，在此文件夹中上传了<code>project.docx</code>，你可以通过<code>http://username.github.io/project/project.docx</code>访问。例如我在主分支中创建了<code>cache</code>文件夹，在其中创建了<code>files</code>又在其中储存了<code>crazysong6.mp3</code>，你可以通过[<code>http://www.computereric.xyz/cache/files/crazysong6.mp3</code>](http://www.computereric.xyz/cache/files/crazysong6.mp3)访问。



#Updating...
