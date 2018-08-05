---
title: hexo
date: 2018-07-31 14:55:27
tags:
---

Create a simple Markdown-based blog for free in 10 minutes :

**Software prerequisites**
- [Npm](https://www.npmjs.com/get-npm)
- [Nodejs](https://nodejs.org/en/download/)
- [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- A Windows, Mac or Linux machine
<!-- more -->

1) Install [Hexo Framework](https://hexo.io/docs/index.html#Install-Git).


2) Setup the blog:

```
$ hexo init {blogname}
$ cd {blogname}
$ npm i
 ```
 
3) Find a [cool theme for Hexo](https://hexo.io/themes/) and clone it in your local themes folder:

```  
$ git clone {theme-github-url} themes/{theme-name}  

```

4) Check the docs of your theme, it may be you have to change some settings to match your liking:

``` 
$ cd themes/{theme-name}
$ vi _config.ym
```

5) Open the `_config.ym` file on the root of the blog (not the theme _config.ym)


``` 
$ cd ../..
$ vi _config.ym
```

6) change the line `theme: ` to match your theme name:

```
theme: {theme-name}


```

7) Update blog info:

``` 
title: Coding tips 
subtitle:
description:
author: Tonino Catapano
language: en
timezone: Europe/Amsterdam

```

8) Create a new blog post:

```
$ hexo new post {your-blog-post-name}

```

9) Edit the Markdown file created under the `source/_posts folder` with you post content!


10) Go on Github and set up a repo called {your_github_username}.github.io


11) Into the settings tab enable the Github pages functionality, eventually settings up your custom
    domain if you own any:


![github pages example](./github_pages.png "screenshot")


12) Set up the blog folder to point at the newly created repo
```
$ git init
$ git SET REMOTE
$ git push

```