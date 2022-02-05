---
title: "로컬환경에서 github blog 작업하기"
excerpt: "ubuntu"
categories: 
  - Blog
tags: 
  - [Github,Blog]
toc: true
toc_sticky: true
author_profile: false
date: 2022-02-02
last_modified_at: 2022-02-02
---
먼저 bundler를 설치해준다.  
gem이 안될경우 ruby설치한다. 

gem install bundler  

이후 로컬 컴퓨터에 있는 surf20.github.io폴더 안에 들어가서 Gemfile이 있는 곳에서 아래 내용을 기입한다. 
bundle install  
bundle exec jekyll serve  

