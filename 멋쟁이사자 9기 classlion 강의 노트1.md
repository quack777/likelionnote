# 멋쟁이사자 9기 classlion 강의 노트1



## 웹기초



### 1.Web & Web Service

 클라이언트 -> Request (갖다 줘 = GET, 처리해줘 = POST)

### 2.웹 서버를 만드는 방법

1.  내 컴퓨터를 서버컴퓨터화 시키기 (로컬환경세팅)

   (e.g. 아파치, IIIS) 장단점 있음

2.  이 세상 어딘가의 서버 컴퓨터 인터넷으로 빌리기 (웹호스팅)

   (e.g. GitHub, AWS c9) 장단점 있음

### 3.HTML [1]

Live Server 단축키 -> ALT + L + O



- 실제 글


1. 글
2. 글을 감싸는 틀 <제목><한 문단> 등등
3. 틀에 붙는 부가설명 (눈사람 사진, www.likelion.net)

-  HTML코드


1. 글
2. 태그
3. 속성

### 4.HTML [2]

 

대원칙! HTML로 꾸미려 들지 말자 -> HTML은 애초에 '꾸미는 언어'가 아님 꾸미는 언어는 CSS!



```>html
<!DOCTYPE html>
<html lang="ko">
<html>

<form action="전송받을 대상">
</form>
```



 html 기본세팅 단축키 : !+tab



### 5.HTML [3]

 리스트 단축키 :  ol 또는 ul > li*숫자

 리스트 -> ol(정렬O), ul(정렬X)



- #### 리스트 태그

```html
<ol>
    <li>순서O</li>
</ol>
<ul>
    <li>순서X</li>
</ul>
```

- #### 아이디 비밀번호 입력 태그

```html
<input type = "text" name = "myid">
```

- #### 긴 문장 쓸 때 사용하는 태그

```html
<textarea cols="높이" rows="넓이"></textarea>
```

- #### 이미지 태그

```html
 <img src = "지수.jpg" height="30" width="20">
```

- #### 선택 태그 

```html
<select>
    <option value="goodday">좋은날</option>
</select>
```

- #### 링크 태그

```html
<a href="링크파일이름">링크 표시되는 문장</a>
```



### 6.Bootstrap

 Bootsrap이란? 

 Bootstrap CDN -> head 태그에 붙혀넣기

```
<!-- 합쳐지고 최소화된 최신 CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap.min.css">

<!-- 부가적인 테마 -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/css/bootstrap-theme.min.css">

<!-- 합쳐지고 최소화된 최신 자바스크립트 -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.2/js/bootstrap.min.js"></script>
```



jQuery 3.x -> head 맨 위에 붙혀넣기

```
<script
  src="https://code.jquery.com/jquery-3.6.0.js"
  integrity="sha256-H+K7U5CnXl1h5ywQfKtSj8PCmoN9aaq30gDh27Xc0jk="
  crossorigin="anonymous"></script>
```



### 7.Github배포

Github : 3+1가지의 기능

1. Code 저장 기능
2. Undo 기능
3. 협업기능
4. **Web Hosting** 기능