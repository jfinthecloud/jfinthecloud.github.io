---
layout: post
title:  "GitHub Pages 教程"
date:   2021-05-30 17:47:45 -0400
#last_modified_at:
lang: zh-Hans
categories: [jekyll, github]
tags: 教程
---

我属于转码吧。我的学历背景是金融和经济。工作经验做过项目经理和业务分析师。学了一点SQL，上了数据分析boot camp转码的。现在做Salesforce顾问，觉得有很多不懂，有很多需要学。想建立博客记录学习。

现在建立博客的选择太多了。研究了一会儿，大概有两类：动态 （dynamic）和 静态（static)。Wordpress是个很受欢迎的动态博客平台。静态网站平台有Netlify, GitHub Pages, Heroku, etc.

<h3>为什么我选择GitHub Pages？</h3>
1. 因为熟悉把。Bootcamp期间，作业和portfolio都是用GitHub。
2. 搭建快！记录笔记的不需要那么多bells and whistles。简单就好。
3. 免费！

<h3>GitHub Pages 教程：</h3>
1. 注册 GitHub
2. 建立仓库(repository).仓库名很重要。必须是 用户名.github.io。比如，我的用户名是 jfinthecloud，我的仓库名是 'jfinthecloud.github.io'。这个仓库名就是你的URL。
3. 进入仓库。点入 Settings。点入 Pages。点入 Choose a Theme。GitHub有12个模板可以选。如果你喜欢其中一个模板，点Select Theme。恭喜！你完成搭建博客啦。

如果看不中这几个模板，Jekyll有不少模板选择，有免费和收费的。Jekyll是什么？是一个博客形态的静态站点生产机器...简单说把纯文本（比如markdown）转换为静态博客网站。

<strong>环境:</strong>
1. 安装 Git（我用 Git Bash）。我用Windows，Mac可能不需要安装。
2. 安装 Ruby
3. 安装 bundler。Terminal输入：gem install bundler
4. 安装 Jekyll。Terminal输入：gem install jekyll bundler
5. Terminal导航到保存博客的文件夹。
6. Terminal输入：git init 用户名.github.io （新建文件夹并且连接到仓库）
7. Terminal输入：cd 用户名.github.io
8. Terminal输入：git checkout --orphan gh-pages （新建branch gh-pages）
9. Terminal输入：jekyll new . (新建jekyll网站)
10. 通过Visual Studio Code打开Gemfile。gem "jekyll" 前面加 #。比如 # gem "jekyll"
11. gem "github-pages", group: :jekyll_plugins 修改成  gem "github-pages", "~> 214", group: :jekyll_plugins
12. 保存Gemfile
13. Terminal导航到仓库文件夹，输入 bundle update
14. Terminal输入：git add .
15. Terminal输入：git commit -m 'Initial GitHub pages site with Jekyll'
16. Terminal输入：git push -u origin gh-pages
17. 回到GitHub网页，进入仓库，点入Settings， 点入Pages，确认Source branch是gh-pages。
18. 换Jekyll模板：[Jekyll](https://jekyllthemes.io/)有很多收费和免费选择。创作者提供用法说明书。

<strong>文章的写法</strong>

Markdown开头加上一段:
<pre><code>
---
layout: post
title:  "Title Goes Here"
date:   2021-05-29 17:47:45 -0400
last_modified_at: 2021-05-30 17:47:45 -0400
lang: zh-Hans
categories: [jekyll, github]
tags: tutorial
---
</code></pre>

<strong>Preview/预览博客</strong>
1. Terminal输入: bundle install
2. Terminal输入：bundle exec jekyll serve
3. 打开浏览器，输入 http://127.0.0.1:4000

关键的都应该记录下来了。谢谢观看。目前还没有开通评论功能。还在考虑Disqus。有评论可以来小红书搜索我：Hello樊爷
