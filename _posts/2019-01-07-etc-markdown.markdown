---
layout: post
title:  "Markdown 문법 정리"
date:   2019-01-08 22:50:00 +0900
categories: etc
---

## 들어가는 글
이 블로그의 글을 작성하거나 깃허브에서 마크다운 문서를 작성하기 위해 markdown 사용법을 정리해두려고합니다.


<br>
* * *
## 마크다운이란?

Markdown은 텍스트 기반의 마크업언어로 2004년 존그루버에 의해 만들어졌으며 쉽게 쓰고 읽을 수 있으며 HTML로 변환이 가능합니다.
특수기호와 문자를 이용한 매우 간단한 구조의 문법을 사용하여 웹에서도 보다 빠르게 컨텐츠를 작성하고 보다 직관적으로 인식할 수 있습니다.
깃헙의 저장소Repository에 관한 정보를 기록하는 README.md는 깃헙을 사용하는 사람이라면 누구나 가장 먼저 접하게 되는 마크다운 문서입니다. 마크다운을 통해서 설치방법, 소스코드 설명, 이슈 등을 간단하게 기록하고 가독성을 높일 수 있다는 강점이 부각되면서 점점 여러 곳으로 퍼져가게 됬습니다.



<br>
* * *
## 마크다운의 장-단점

### 1. 장점
	1. 간결하다.
	2. 별도의 도구없이 작성가능하다.
	3. 다양한 형태로 변환이 가능하다.
	3. 텍스트(Text)로 저장되기 때문에 용량이 적어 보관이 용이하다.
	4. 텍스트파일이기 때문에 버전관리시스템을 이용하여 변경이력을 관리할 수 있다.
	5. 지원하는 프로그램과 플랫폼이 다양하다.
### 2. 단점
	1. 표준이 없다.
	2. 표준이 없기 때문에 도구에 따라서 변환방식이나 생성물이 다르다.
	3. 모든 HTML 마크업을 대신하지 못한다.


<br>
* * *
## 마크다운의 사용법



### 1.헤더Headers

This is an h1
===
    this is an h1
	===
This is an h2
---
    this is an h2
    ---
# this is an h1
	## this is an h1
## this is an h2
	## this is an h2
### this is an h3
	### this is an h3
####this is an h4
	#### this is an h4
##### this is an h5
	##### this is an h5
###### this is an h6
	###### this is an h6
<br>


### 2.BlockQuote

> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.

```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```

<br>
이 안에는 다른 마크다운 요소를 포함할 수 있습니다.
> ### This is a H3
> * List
>	####code

```
> ### This is a H3
> * List
> ###code
```
<br>


## 3.목록

**순서있는 목록(번호)**

1. 첫번째
2. 두번째
3. 세번째

```
1. 첫번째
2. 두번째
3. 세번째
```
<br>

**순서없는 목록(글머리 기호)**

* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑

```
* 빨강
  * 녹색
    * 파랑

+ 빨강
  + 녹색
    + 파랑

- 빨강
  - 녹색
    - 파랑
```
<br>

**혼합해서 사용하는 것도 가능하다**

* 1단계
    - 2단계
    	+ 3단계
			= 4단계

```
* 1단계
    - 2단계
    	+ 3단계
            = 4단계
```


## 4. 코드


**4개의 공백으로 시작**

This is a normal paragraph:

    This is a code block.
end code block.


```
This is a normal paragraph:

    This is a code block.
end code block.
```

<br>

**\```로 시작 \```로 끝**

```
i am first row
and i am second row.
```

```
(\는 무시해주세요)
\`\`\`
i am first row
and i am second row.
\`\`\`
```


## 5. 수평선

```
* * *
***
*****
- - -
```

* * *
***
*****
- - -


## 6. 링크

**참조링크**
```
Link: [Google][googlelink]
[googlelink]: https://google.com "Go google"
```
Link: [Google][googlelink]
[googlelink]: https://google.com "Go google"

**인라인 링크**
```
Link: [Google](https://google.com, "google link")
```
Link: [Google](https://google.com, "google link")

**자동연결**
```
<http://example.com/>
<address@example.com>
```
<http://example.com/>
<address@example.com>


## 7. 강조
```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
++underline++
~~cancelline~~
```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
++underline++
~~cancelline~~

## 8. 이미지
local path 도 가능합니다
사이즈 조절 기능은 없기 때문에 ```<img width="" height=""></img>```를 이용한다.
```
![석촌호수 러버덕](http://cfile6.uf.tistory.com/image/2426E646543C9B4532C7B0)
![석촌호수 러버덕](http://cfile6.uf.tistory.com/image/2426E646543C9B4532C7B0 "RubberDuck")
```
![석촌호수 러버덕](http://cfile6.uf.tistory.com/image/2426E646543C9B4532C7B0)
![석촌호수 러버덕](http://cfile6.uf.tistory.com/image/2426E646543C9B4532C7B0 "RubberDuck")

<br>
* * *


## 참고문서
아래 마크다운 markdown 작성법 링크에서 대부분 가져와 제가 필요한 부분만 정리해놨습니다.

[마크다운 markdown 작성법](https://gist.github.com/ihoneymon/652be052a0727ad59601#file-gistfile1-md)
[마크다운 문법 간략 정리](https://blog.ayukawa.kr/archives/1290)
