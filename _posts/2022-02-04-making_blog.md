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
{% gist surf20/7b19aeebab8d1147a9ea4ee96aa8303d %}

# Github blog 만들기  
Github 사이트에서 계정을 만든다.  
Github.io>_config.yml로 이동한다.  
다음과 같이 _pages 내용 추가한다.  

defaults:    
  // _pages                        : 해당 하단 영역이 새로 추가되었습니다.  
  - scope:  
      path: "_pages"  
      type: pages  
    values:  
      layout: single  
      author_profile: true  

수정 파일 : github.io 폴더 > _data 폴더 > navigation.yml  
만약 Category 와 Tag를 만든다면  
다음과 같이 수정한다.  

main links  
main:  
   title: "Home"  
   url: "/"  
  - title: "Introduce"  
    url: /about/  
  - title: "Category"  
    url: "/categories/"  
  - title: "Tags"  
    url: /tags/  
 
 _pages 폴더를 생성한후 category-archive.md, tag-archive.md파일을 만들자.  
 아래내용으로 작성하자  
{% gist surf20/906e9529b7f4fc86b4f88cbdc474819d %}


# 블로그 글 작성하기  
_posts 폴더아래 yyyy-mm-dd-Github블로그만들기.md 작성한다.  
내용 적기전 머리말엔 다음 포함한다.  
{% gist surf20/3320a95addb2b6198edc4124fb396572 gist %}

# 나의 블로그에 search 넣기  
Github.io>_config.yml이동하여 아래 내용대로 수정한다.  
search: true  

# 나의 블로그에 코딩 집어넣기
Gisthub의 화면 좌측 상단에 + 클릭 > create gist를 클릭한다.
문서명.yml
내용 기입후 create한다. > embed 링크 복사하면 다음과 같이 될것이다.  
<script src="https://gist.github.com/surf20/3320a95addb2b6198edc4124fb396572.js"></script>
이 포맷에서 surf20/3320a95addb2b6198edc4124fb396572을 {%gist %}안에 gist 다음위치에 복사해서 넣어준후 posting할 내용에 링크를 paste해주면  


