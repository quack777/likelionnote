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



# HTML/CSS

### 1. Intro

**HTML** (구조): HyperText Markup Language -> 

웹 페이지의 구조 혹은 데이터 작성을 위한 마크업 언어

- Hyper Text : 하이퍼 텍스트 -> 링크를 이용
- Markup Language : 마크업 언어 -> 태그(마크, 표시)를 이용하여 문서나 데이터의 구조를 명시하는 언어



**CSS**(스타일) : Cascading Style Sheets -> 

웹 페이지에 관한 다양한 스타일 들을 정의

- Style Sheets : 웹 페이지의 스타일과 관련된 모든 것을 정해둠



**Javascript**(동작) : 웹을 이용하는 유저와 상호작용 하기 위한 기능을 추가할 때 쓰는 언어



### 2. HTML 기초

- **태그** : 내용을 나누고 어떤 역할을 하는지 구조를 정의
- **시작태그** : 컨텐츠의 시작을 표시
- **종료태그** : 컨텐츠의 끝을 표시



- **<!DOCTYPE html**/ : 문서 형식을 정의

- **meta charset="utf-8"** : 문서와 관련된 정보를 담음

  

### 3. 텍스트와 관련된 태그

- **제목 태그** : 제목을 나타내고 싶을 때 사용 중요도에 따라 1~6까지 씀

- **p 태그** : 엔터를 눌러도 엔터기능 먹히지 않음

- **br 태그** : 엔터 기능 , 빈태그

- **pre 태그** 

- **strong 태그** : 굵게

- **em 태그** : 기울이게

- **sub 태그** : 아래에 내리기

- **sup 태그** : 위로 올리기

- **ins 태그** : 밑줄

- **del 태그** : 취소선

  

### 4. 링크 태그

- **a 태그 , href **

```html
<a href="www.google.com">구글</a>
```



- **URL(Uniform Resource Locator)** : 인터넷에서 HTML페이지, CSS문서, 이미지 등 자원(Resource)의 위치를 나타냄

- **절대 URL** : 접근하는 최초 시작점부터 경유한 경로를 모두 기록하여 리소스의 위치를 나타냄
- **상대 URL** : 기준점을 기준으로 상대적인 경로를 기록하여 리소스의 위치를 나타냄



- **target :** 클릭으로 링크를 열 때 어디에 오픈 할 것인지 정하는 속성
- **target="_self" :** 현재 탭에서 링크를 여는 속성
- **target="_blank" :** 새 탭(창)에서 링크를 여는 속성

###  

### 5. 멀티미디어와 관련된 태그

- **img태그** (사이즈는 CSS를 사용하는 것 권장)

```html
<img src="이미지 url" alt="사진 설명">
```

- **alt="사진설명"** : 불러올 이미지가 없거나 불러오는데 실패했을 경우 대신 표시되는 문장 alternative text(대체 문구)의 약자



**TIP. 유튜브 영상 넣는 방법** : 해당 영상 -> 공유 -> 퍼가기 -> 코드 복붙



### 6. 테이블과 리스트

#### 테이블

- **table :** 표 전체를 감싸는 태그

- **tr :** 표에서 행을 구분하는 태그

- **th :** 표의 행 내부에 제목 셀을 담는 태그

- **td :** 표의 행 내부에 데이터 셀을 담는 태그

- **rowspan="숫자"** : "숫자"만큼 셀이 행을 점유

- **colspan="숫자"** : "숫자"만큼 셀이 열을 점유

  

#### 리스트

**1.ol : 순서o**

- start="숫자" : 리스트가 시작하는 숫자를 정함
- type="문자" : 순서를 시작하는 문자를 정함
- reversed : 순서를 반대로 시작 다른 속성과 달리 키(key)만 써서 사용

```html
<ol>
    <li>아이템</li>
</ol>
```

**2.ul : 순서x**

```html
<ul>
    <li>아이템</li>
</ul>
```

value="숫자" : 해당하는 리스트 아이템의 번호를 지정



### 7. 폼 태그

- **form 태그** : 폼에 포함되는 다양한 입력 양식 태그 들을 감싸줌

- **action** : 데이터를 보낼 URL을 지정

- **method** : 보내는 방식을 지정
  -  method="get" : 데이터를 URL 끝에 붙여 눈에 보이게 보냄
    - 특징 : 데이터 조회 만을 목적으로 할 때 주로 쓰임
  -  method="post"
    - 특징 : 서버에 있는 데이터를 쓰거나 수정, 삭제 할 때 주로 사용

- **input** : 사용자에게 입력을 받기 위해 사용되는 태그, 빈 태그

  - type="text" : input 태그의 종류를 결정
  - namd="id" : input태그 중 같은 타입과 구분되는 이름을 결정
  - value="eunchong" : 실제 할당되는 값, 우리가 데이터를 넣으면 이 속성에 값이 들어감. 초기값처럼 둘 수 있음

- **lable** : 해당하는 라벨을 클릭 시 input태그가 활성화 됨

  ```html
  <input id="password">
  <labe for="password">비밀번호: </label>
  ```

- **div** : 태그 들을 구분 짓고 나누기 위해 사용되는 태그 division의 약자

- **select** : 여러 개의 선택지를 제시하고 싶을 때 씀

  - selcet **name="gender"** : input태그의 name속성과 동일하게 작동
  - option **value="male"**>남성<option : input 태그에서 입력한 값과 동일한 역할

- **textarea** : 한 번에 많은 글을 입력 받을 때 사용
  - cols : 글자 수
  - rows : 줄 수

- **button** : input태그의 버튼타입과 동일하게 버튼을 생선

  ```html
<button type="submit">회원가입</button>
  ```
  
  ```html
  <input type="button" value="회원가입">
  ```
  
  위 두개 같음