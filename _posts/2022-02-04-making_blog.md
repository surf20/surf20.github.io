---
title: "Github블로그 만들기"
excerpt: "minimal mistakes"
categories: 
  - Blog
tags: 
  - [Github,Blog]
toc: true
toc_sticky: true
author_profile: false
date: 2022-02-05
last_modified_at: 2022-02-05
---

# 로컬 컴퓨터에서 커밋하기  
{% gist surf20/7b19ae
ebab8d1147a9ea4ee96aa8303d %}

# Github blog 만들기  
Github 사이트에서 계정을 만든다.  
Github.io>_config.yml로 이동한다.  

{% gist surf20/a85dd932264eeec728675f1c684b3de6 %}

# 블로그 글 작성하기
_pages 폴더를 생성한후 category-archive.md, tag-archive.md파일을 만들자.  
 아래내용으로 작성하자 
 
{% gist surf20/906e9529b7f4fc86b4f88cbdc474819d %}

# 나의 블로그에 search 넣기  
Github.io>_config.yml이동하여 아래 내용대로 수정한다.  

search: true  

# 나의 블로그에 코딩 집어넣기
Gisthub의 화면 좌측 상단에 + 클릭 > create gist를 클릭한다.
문서명.yml
내용 기입후 create한다. > embed 링크 복사하면 다음과 같이 될것이다.  
해당 링크에서 surf20/3320a95addb2b6198edc4124fb396572을 {%gist %} 안에 gist 다음위치에 복사해서 넣어준후 posting할 내용에 링크를 paste해주면




