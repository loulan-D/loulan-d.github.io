---
layout: post
title: "Deploy Octopress"
date: 2018-10-12 17:12:51 +0800
comments: true
categories: 

---

#### 1. Install Ruby on Ubuntu 

##### apt(Debian or Ubuntu )    Debian GNU/Linux  and Ubuntu use the apt package manager. You can use it like this:

```shell
$ sudo apt-get install ruby-full
```

##### check the install

```shell
$ ruby -v 
```

------

#### 2. Install Octopress

#####    check the git 

```git
git --version
```

#####    git clone octopress

```git
git clone git://github.com/imathis/octopress.git octopress 
```

#####    install others

```
cd octopress
gem install bundler
rbenv rehash
bundle install 
rake install
```

------

#### 3. Octopress deploy to Github Pages

1. rake setup_github_pages

2. rake generate 

3. http://localhost:4000/rake deploy

4. github

   > ##### git add .
   >
   > ##### git commit -m 'initial source commit'
   >
   > ##### git push origin source     ----- 将博客文件的原始文件提交到另外一个source 分支上

#####  

------

#### 4. Create new Post

> ##### rake new_post['title']
>
> ##### rake generate
>
> ##### rake preview
>
> ##### rake deploy
>
> ##### git commit -a
>
> ##### git push origin source

------



#### Reference

​	https://www.jianshu.com/p/0c21051317fe

​	https://www.jianshu.com/p/40d90a71cab4

​	https://www.jianshu.com/p/dd7a56d05fb5

