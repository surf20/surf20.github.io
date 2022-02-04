---
title: "Github 블로그 만들기"
excerpt: "블로그 만들기 기억하기"
categories: 
  - Blog
tags: 
  - [Github,Blog]
toc: true
toc_sticky: true
author_profile: false
date: 2022-02-05
---

# 로컬 컴퓨터에서 커밋하기  
git init  
git remote add origin https://github.com/surf20  
git pull origin master  
git add *  
git commit -m "added"  
git push origin master  

# Github blog 만들기  
Github 사이트에서 계정을 만든다.  
Github.io>_config.yml로 이동한다.  
다음과 같이 추가한다.  

defaults:  
  # _posts  
  - scope:  
      path: ""  
      type: posts  
    values:  
      layout: single  
      author_profile: true  
      read_time: true  
      comments: # true  
      share: true  
      related: true  
  
  # _pages                        : 해당 하단 영역이 새로 추가되었습니다.
  - scope:  
      path: "_pages"  
      type: pages  
    values:  
      layout: single  
      author_profile: true  

수정 파일 : github.io 폴더 > _data 폴더 > navigation.yml  
만약 Category 와 Tag를 만든다면  
다음과 같이 수정한다.  

# main links  
main:  
  #- title: "Home"  
  #  url: "/"  
  - title: "Introduce"  
    url: /about/  
  - title: "Category"  
    url: "/categories/"  
  - title: "Tags"  
    url: /tags/  
 
 _pages 폴더를 생성한후 category-archive.md, tag-archive.md파일을 만들자.  
 아래내용으로 작성하자  

---  
title: "Posts by Category"  
layout: categories  
permalink: /categories/  
author_profile: true  
---  

---  
title: "Posts by Tag"  
permalink: /tags/  
layout: tags  
author_profile: true  
---  

# 블로그 글 작성하기  
_posts 폴더아래 yyyy-mm-dd-().md 작성한다.  
---  
title: "블로그 포스팅 첫날!!"  
excerpt: "조금씩 Github에 익숙해지고 있음"  
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
# search 넣기  
Github.io>_config.yml로 이동한다.  
search: true  

