---
layout: post
title: "deploy-octopress"
date: 2018-10-12 19:45:16 +0800
comments: true
categories: Github Pages

---

### Octopress Deploy to Github Pages



#### 1. Install Ruby on Ubuntu 

```python
tar -zxf ruby-2.5.0.tar.gz

cd ruby-2.5.0

./configure --prefix=/usr/local/ruby

make

sudo make install

sudo gedit /etc/profile

export RUBY_HOME =/usr/local/software/ruby-2.5.0

export PATH=${RUBY_HOME}/bin:$PATH

source /etc/profile

ruby -v          
```

 

------

#### 2. Install Octopress

##### check the git 

```
git --version
```

##### git clone octopress

```
git clone git://github.com/imathis/octopress.git octopress 
```

##### install others

```
cd octopress
gem install bundler
rbenv rehash
bundle install 
rake install
```

------

#### 3. Octopress deploy to Github Pages

```python
rake setup_github_pages

rake generate 

rake deploy

github

git add .

git commit -m 'initial source commit'

git push origin source    
```

#####  

------

#### 4. Create new Post

```ruby
rake new_post['title']

rake generate

rake preview

rake deploy

git commit -a

git push origin source
```



#### Reference

​	https://www.jianshu.com/p/0c21051317fe

​	https://www.jianshu.com/p/40d90a71cab4

​	https://www.jianshu.com/p/dd7a56d05fb5

