> [我搭建的博客](https://penghaos.github.io/2016/08/17/%E5%A6%82%E4%BD%95%E5%9C%A8github%E4%B8%8A%E7%94%A8jekyll%E6%90%AD%E5%BB%BA%E5%8D%9A%E5%AE%A2.html)

首先，你要知道什么是github。

先在github上注册一个账号：

> [github传送门](https://github.com/)

**sign up** 后，你会有个用户名，比如lin。

添加一个新仓库：点击`New repository`，取名**lin.github.io**（一定要是这个名字否则不会生成网站——用户名.github.io）

![github1](https://github.com/penghaos/penghaos.github.io/blob/master/public/img/posts/github1.png?raw=true)

点击如图的最右边的`Settings`，向下翻，找到这个界面

![github2](https://github.com/penghaos/penghaos.github.io/blob/master/public/img/posts/github2.png?raw=true)

点击`Launch auotmatic page generator` 自动生成博客。

此时你需要懂一点**git**的指令：

```
git clone git@github.com:lin/lin.github.io.git 
```

>[git教程](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/00137396287703354d8c6c01c904c7d9ff056ae23da865a000)

克隆下来后，你在自己的电脑上，也就是`c:/用户/电脑名` 会有个文件夹`lin`

，`lin`里面有个文件夹叫`_posts`，是存放文章的地方。

以后只要往`_posts`中放入文章，并推送到githu上，就可以自动更新博客了。

文章都是用markdown格式写成的，如果你不知道markdown格式，请看教程：

>- [markdown教程](http://www.yangzhiping.com/tech/r-markdown-knitr.html)
- [為什麼文科生也該用markdown寫作?](http://www.douban.com/note/221187015/)

 注意，在每篇文章开头要加上一段文字，是YAML语言：

```
 layout: post
 title: 标题
 date: 2016-08-17
 ```

（另一个注意事项：YAML的缩进要相同，比如各行语句的`冒号：`与后面文字间的**空格数**要**相同**）

每篇文章的命名方式为`yyyy-mm-dd-文件名.md`的格式，比如：`2016-08-17-如何在github上建立博客.md`

将文章放入`_posts`文件夹后，接着用git推送：

```
git add -A
git commit -m "我添加了一个文件"
git push origin master
```

博客的文章更新了！

------

如果你对github提供的博客模版不满意的话，你可以上网找jekyll的模版，比如搜索`jekyll 模版`

>- [jekyll](http://jekyllthemes.org/)
- [jekyll2](http://jekyllthemes.io/)

下载压缩包后，解压。

删除原来`lin`里面的所有内容，放入解压后的文件。

试着同步本地到远程仓库。

```
git fetch
git pull origin
git add -A
git commit -m "我要推送了，别拦我！"
git push origin master
```

你可能会碰到一些问题，自己谷歌一下，前人基本都已经给出了答案。

------
