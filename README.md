# test.github.io
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
- **name** : form의 이름, 서버로 보내질 때 이름의 값으로 데이터 전송
- **autocomplete** : 자동완성. on으로 하면 form전체에 자동 완성 허용



#### form내부의 태그들

- **input** : 사용자에게 입력을 받기 위해 사용되는 태그, 빈 태그

  - **type**="text" : input 태그의 종류를 결정
    - ex. text, password, button, submit, reset, radio, checkbox, file, hidden
  - **namd**="id" : input태그 중 같은 타입과 구분되는 이름을 결정
  - **value**="eunchong" : 실제 할당되는 값, 우리가 데이터를 넣으면 이 속성에 값이 들어감. 초기값처럼 둘 수 있음

- **lable** : 해당하는 라벨을 클릭 시 input태그가 활성화 됨

  ```html
  <input id="password">
  <labe for="password">비밀번호: </label>
  ```

- **div** : 태그 들을 구분 짓고 나누기 위해 사용되는 태그 division의 약자

- **select** : 여러 개의 선택지를 제시하고 싶을 때 씀. 선택 항목은 option으로

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



### 8. CSS기초

1. CSS기초 문법

   - **선택자(Selector)** : 스타일을 적용하고자 하는 html요소를 선택하는 역할

   - **속성(Property)** : 지정할 스타일의 속성 이름에 해당

     ​							  속성: 값;이 한 단위

     ​							  ;(세미 콜론)을 이용하여 구분

   - **값(Value)**  : 키워드나 특정 단위를 이용하여 원하는 스타일을 적용 속성(Property)와 쌍을 이룸

   

   - **선언 블록(Declaration block)** : 중괄호 안에 있는 한 블록. {} --> 구분
   - **선언(Declaration)** : 속성과 값 한 쌍을 가르킴 ;세미콜론 필수

   

   2.HTML에 CSS를 적용하는 방법

   - **Link style** : HTML에 외부에 있는 CSS파일을 불러옴
   - **Embedding style** : HTML의 head에 style를 이용하여 CSS를 작성
   - **Inline style** : HTML요소에 직접 style 속성(Attributes)을 이용하여 CSS를 작성 	

   

### 9.선택자

**선택자(Selector)** : 스타일을 적용하고자 하는 html요소를 선택하는 역할 

-> ex) h1, p, span, div, a 등등 **일반적인 태그** 사용가능

```css
h1,p{
	color: red;
}
```

여러 개의 선택자를, 를 이용하여 스타일을 한번에 지정 가능



#### 단순 선택자 (타입, 클래스, 아이디, 전체, 속성)

- **타입 선택자(Type Selector)** : 해당 **태그**를 가지는 **모든** 요소에 스타일을 적용
- **아이디 선택자(Id Selector)** : Id로 스타일을 적용 해당 Id 하나에 적용(Id는 단 하나)
  - #main { color: red; }
  - 아이디(Id) : HTML 문서 내에서 동일한 아이디는 존재할 수 없음 다른 요소와 구분되는 점을 만들어줌
- **클래스 선택자(Class Selector)** : 클래스 이름으로 스타일을 적용 **같은 클래스 이름**이면 **모두** 적용
  - .main{ color : red; }
  - 클래스(Class) : 비슷한 특징을 갖는 요소를 지정하여 묶을 수 있음 여러 번 사용이 가능
- **전체 선택자(Universla Selector)** : **모든 요소**에 스타일을 적용 모든 요소에 적용하기 때문에 속도 저하 가능성이 있음
  - *{color : red;}
- **속성 선택자(Attribute Selector)** : 특정 속성을 소유하는 모든 요소에 스타일을 적용
  - 선택자[속성명="속성값"]{ color : red; }
  - a[target="_blank"] {color : red;}

#### 복합 선택자

![image-20210724151349395](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20210724151349395.png)

- **자식 선택자(Child Selector)** : **선택자A**의 모든 자식 중 **선택자B**와 일치하는 요소 선택                                   (선택자A 중 선택자B선택)

  - 선택자A > 선택자B { color: red; }
  - article > p { color : red; }

- **후손 선택자(Descentdant Selector)** : **선택자A**의 모든 후손 중 **선택자B**와 일치하는 요소 선택

  - 선택자A 선택자B { color:  blue; }
  - article p { color : blue; } 

- **pseudo 클래스(가상의 클래스)** : 요소의 특별한 상태를 지정할 때 씀

  - 예시 : :link , :visited, :hover 그 외

  - 선택자 : pseudo-class {

    ​	속성 : 속성값;
  
    }
  
    - :link :방문하지 않은 링크일 경우
    - :visited :방문한 링크일 경우
    - :hover :요소에 마우스가 올라와 있을 경우 
  
    

### 10.값과 단위

#### 		숫자값과 백분율

- 1px = 1/96 in (**절대길이**)
- em rem -> **상대적인 길이**
- **em** : 현재 스타일이 지정된 요소의 font-size기준
- **rem** : 최상위 요소의 font-size기준 (**rem쓰는 것 권장**)
- em과 rem을 쓰는 이유 : 웹을 피시와 모바일에서 보고 기기마다 사이즈가 다르니까 상대길이 사용
- 1em(1rem)의 크기 = 기준 font-size *1em(1rem)

​			ex) 10em(rem) = 16px * 10 = 160px

- **%(퍼센트)** : 상대 길이, 보통 이미지나 레이아웃의 너비나 높이를 지정할 때 씀

  

  #### 색상
  
  - **hex code** : #~
  - **rgb** : red, blue
  - **hsl**
  
  

### 11.텍스트와 관련된 프로퍼티

#### 			폰트와 관련된 프로퍼티

- ex : font-size, font-family, font-style, font-weight

- **font-family** : 'Cute Font', Arial, cursive;

- **font-style** : normal(기본 값), italic(디자인된 폰트에 적용), oblique(기울임 글꼴)

- **font-weight** : 100, 200, normal(400), bold(700) 등등

- font : oblique 900 35px; -> 한 번에 적용 가능, 띄어쓰기로 구분

  

  #### 텍스트 정렬관 관련된 속성 (자기 자신을 기준으로 정렬)

- **text-align** : 텍스트를 좌,우,중앙 정렬함

- **line-height** : 문장 사이의 간격을 조정함

- **letter-spacing** : 글자와 글자 사이의 간격을 조정함, 자간

- **text-indent** : 문단의 시작부에 들여쓰기를 함

  

### 12.박스

#### 		박스 모델 개념

- HTML의 **모든 요소**는 **상자(Box)형태**를 가진다.

<img src="C:\Users\82108\Desktop\멋쟁이사자\화면 캡처 2021-01-23 031036.jpg" style="zoom:50%;" />

#### Content와 Border

- 컨텐트 사이즈는 width와 height로 지정
- border는 border-style, border-width, border-color
- **border-radius** : px은 반지름의 길이, 타원형 가능 값에 px 두개 집어넣으면 됨



#### 	padding과 margin

- 위 아래 다른 요소에서 마진을 적용하면 마진끼리 함께 공존하지 않음

  -> 마진 상쇄(Margin Collapse)  -> 큰 쪽마진을 기준으로 작은 거는 삭제 됨

- **box-sizing : content-box**; -> 기본 박스 사이즈 

  -> width(height) = content size

- **box-sizing : border-box;**  -> border까지 기준 박스 사이즈

  -> width(height) = content size + padding + border



### 13.위치와 관련된 프로퍼티[1]

#### 	HTML 요소

1. block element : 항상 새로운 줄에서 시작 항상 width 100%를 가지고 있음

2. inline element : 필요한 만큼의 너비만 가짐. 즉, 요소의 content크기만큼만 너비를 가짐

   

#### 			display

- **display** : 요소가 보여지는 방식을 지정

- **display : block;**(width 100%)

  ex. div, h1~6, p, header, section

  *width, height, margin, padding 가능

- **display : inline;**

  ex. a, span, img

  *width, height, margin-top, margin-bottom 불가능

- **display : inline-block;** : width, height, margin-top, margin-bottom 가능

- **display: none;** : 해당 요소 출력이 되지 않음

  ![image-20210725172828791](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20210725172828791.png)

  

  #### position

- **static** : 기본값! 좌표 프로퍼티를 쓸 수 없음

- **relative** : 상대위치. **기본 위치를 기준으로 좌표를 사용**함. 좌표 프로퍼티 사용 가능

  여기에서 기본 위치를 기준으로라는 말은 원래 있어야할 위치를 기준으로 이동한다는 의미

  원래에 block요소처럼 작용

- **absolute** : **부모나 조상 중 relative, absolute, fixed가 선언된 곳을 기준으로 좌표 프로퍼티 적용**

   넓이가 inline요소처럼 보임 -> 이렇게 보인다고 width, heigth 적용 안된다고 생각하지 않기

- **fixed** : 보이는 화면을 기준으로 좌표 프로퍼티를 이용하여 위치를 고정

  스크롤해서 밑으로 내려도 그대로 고정하고 싶을때 사용

- **z-index** : 숫자값이 클수록 전면에 출현

  이미지나 content가 겹칠 때 앞으로 배치하고 싶을때 사용



### 14.위치와 관련된 프로퍼티[2]

#### 		flexbox

- **flexbox** : 특별한 계산 없이 정렬(가로/세로 정해진 방향으로 정렬)

- flex container(부모 요소 <-display : flex 추가)

  #### 부모요소

- **flex-direction** : flex 컨테이너 안의 item들의 방향을 정함

- **flex-wrap** : flex 아이템이 flex 컨테이너를 벗어 났을 때 줄을 바꾸는 속성

- **justify-content** : flex-direction으로 정해진 방향을 기준으로 수평으로 item을 정렬하는 방법을 정함

- **aling-items** : flex-direction으로 정해진 방향을 기준으로 수직으로 item을 정렬하는 방법을 정함

- **aling-content** : flex-direction으로 정해진 방향을 기준으로 수직으로 **여러 줄인** item을 정렬하는 방법을 정함

  #### 자식요소

- **flex-grow** : flex 아이템의 확장과 관련된 속성, 기본 0

- **flex-shrink **: flex 아이템의 축소와 관련된 속성, 기본 1

- **flex-basis** : flex 아이템의 기본 크기를 결정함, 기본 auto

- **flex** : flex-grow, flex-shrink, flex-basis의 축약형

  

### 15.상속과 우선순위

#### 	상속

​		모든 CSS 프로퍼티가 상속되는 것은 아님

​		https://www.w3.org/TR/CSS21/propidx

​		margin: inherit; -> 상속가능



#### 		우선순위

- **cascading** : 적용 우선 순위
  - 중요도 : 어디에 선언되었는지에 따라서 우선순위 달라짐
    1. head태그 내의 style
    2. head태그 내의 style태그 내의 @import문
    3. link태그로 연결된 css
    4. link태그로 연결된 css내의 @import
    5. 문브라우저 디폴트 스타일시트
  - 명시도
    1. !important
    2. 인라인 스타일
    3. 아이디 선택자
    4. 클래스, 속성, 가상 클래스 선택자
    5. 태그 선택자
    6. 전체 선택자
    7. 상속



### 16. Bootstrap

​	

## Django Settings

### 1. 오리엔테이션

1. 개발은 혼자 하지 않는다.
2. 보안
3. 개발자는 반드시 실수를 한다.



### 2. 터미널 사용법

- **터미널이란?** CLI를 GUI환경에서 사용할 수 있게 하는 것

- **CLI** : Command Line Interface

- **GUI** : Graphic User Interface

  단점

  1. 처음 지정된 기능 밖에 사용 불가
  2. 조작 속도가 CLI에 비해 늦은 경우가 있음

- 특수한 디렉터리

  1. **Home(~)** : 터미널 구동 시 처음 위치하는 디렉터리
  2. **Working directory(.)** : 작업중인 현재 위치
  3. **Root directory(/)** : 모든 디렉터리의 시작점
  4. **상위 디렉터리(..)**
  5. **하위 디렉터리**
  6. **절대 경로** : 루트(/)에서부터 시작. 항상 표현방법이 같다.
  7. **상대 경로** : 현재(.)에서부터 시작. 현재 위치에 따라 다르다.

- 외워야 할 명령어 : pwd, man, ls, cd, clear

- **명령어 구조** : 명령어 [옵션] [인자...]

  - **옵션** : "-"로 시작해서 영문 대소문자로 구성. 명령어의 기능을 구체화. 명령어에 따라 없을 수도 있다. ex) ls-l, ls-a, ls-al, ls-la
  - **인자** : 명령어의 수행시 대상이 될 파일이나 디렉터리 명령어에 따라 필요 없을 수도 있고 필수일 수도 있다.  ex) cp [인자1] [인자2]

- **명령어**

  - pwd : Print Working Directory. 현재 위치를 알려준다.
  - man : manual. 명령어 설명서. man[알고싶은 명령어]
  - ls : list. 디렉터리의 목록을 보여준다.
    1. 옵션 a : 숨김파일까지 보여줌
    2. 옵션 l : 상세하게 보여줌
    3. 옵션 F : 파일인지 디렉터리인지 알려줌
  - cd : change Directory. 현재 위치를 이동해줌. cd[이동하고 싶은 위치]
  - clear : 터미널 청소기



### 3. Django 시작하기

1. 프레임워크를 쓰면 개발 속도가 빠르다.
2. 개발 현장에선 한 프로젝트에 여러 라이브러리와 프레임워크를 동시에 사용한다.



- **Django 사용하는 방법**
  1. python -m venv [가상환경명]
  2. source [가상환경명]/bin/activate . source [가상환경명]/Script/activate
  3. pip install django



## Python

### 1. Class

​	![화면 캡처 2021-07-17 184510](C:\Users\82108\Desktop\markdown\화면 캡처 2021-07-17 184510.jpg)

- **클래스**(class) : 똑같은 무엇인가를 계속해서 만들어 낼 수 있는 설계 도면(과자 틀)
- **객체**(object) : 클래스로 만든 피조물(과자 틀을 사용해 만든 과자)를 뜻한다
- 객채와 인서트스의 차이
  - 클래스로 만든 객체를 인스턴스라고도 한다. 그렇다면 객체와 인스턴스의 차이는 무엇일까? 이렇게 생각해 보자. a = Cookie() 이렇게 만든 a는 객체이다. 그리고 a 객체는 Cookie의 인스턴스이다. 즉 인스턴스라는 말은 특정 객체(a)가 어떤 클래스(Cookie)의 객체인지를 관계 위주로 설명할 때 사용한다. "a는 인스턴스"보다는 "a는 객체"라는 표현이 어울리며 "a는 Cookie의 객체"보다는 "a는 Cookie의 인스턴스"라는 표현이 훨씬 잘 어울린다.
- **메서드**(Method) : 클래스 안에 구현된 함수
- **생성자**(Constructor) : 객체가 생성될 때 자동으로 호출되는 메서드
- **상속**(Inheritance) : "물려받다"라는 뜻으로, "재산을 상속받다"라고 할 때의 상속과 같은 의미
  - class 클래스 이름(상속할 클래스 이름)
- **메서드 오버라이딩**(Overriding, 덮어쓰기) : 부모 클래스(상속한 클래스)에 있는 메서드를 동일한 이름으로 다시 만드는 것

## Django

### 1. MTV패턴

- 복습

  -가상환경

  가상환경 만들기 : python -m venv [가상환경명]

  가상환경 실행 : source [가상환경명]/Script/activate

  django설치 : pip install django

  project 만들기 : django-admin startproject [프로젝트 이름]

  서버 기동하기 : python manage.py runserver

- **MTV**(model, template, view)
  
  - Template : 사용자가 보이는 영역, HTML, CSS 템플릿 언어
  - Model : DataBase(DB)
  - View : 데이터를 처리하는 곳 MTV중에서 핵심



- 코딩 공부할 때 알아야 할 꿀팁
  - 개발은 혼자 하지 않는다
  - 보안
  - 개발자는 반드시 실수를 한다



### 2. Django 실습[1]

- 실습
  1. 가상환경 만들기
  2. 프로젝트 만들기
  3. 앱 만들기
  4. 프로젝트/settings.py에서 앱 설치했다고 코드 작성해주기
     - firstapp.apps.FirstappConfig
     - 앱이름.apps.앱이름Config
  5. 앱에 templates폴더 만들고 html 파일 만들기
  6. view 제작
  7. url연결 
     - from firstapp import views
     - path('',views.wellcome, name="wellcome")
     - 여기서 '',는 서버를 기동시키고 첫 페이지가 wellcome이라는 뜻

- 에러의 이유
  1. 오타 !!!
  2. 저장 안함

- **APP** : Django프로젝트를 이루는 작은 단위

  ![화면 캡처 2021-07-20 175013](C:\Users\82108\Desktop\markdown\화면 캡처 2021-07-20 175013.jpg)

  각각의 서비스 별로 분류한 것

- 웹사이트 구동 순서
  
  1. 사용자가 서버에 요청
  2. 서버의 view는 model에게 요청에 필요한 데이터를 받음
  3. view는 받은 데이터를 적절하게 처리해서  template으로 넘김
  4. template은 받은 정보를 사용자에게 보여줌
  
- 복습

  -앱 제작 순서

  1. App을 생성
  2. Template 제작
  3. View 제작
  4. URL연결

- 템플릿 언어 : html에서 파이썬 변수와 문법을 사용하게 해주는 언어

  ex. {%for word in wordDict%} ... {%endfor%}, {{변수명}}

  

### Django 실습[2]

### 3. Git 사용법

- github 레파지토리
  1. 깃허브 들어가서 레파지토리 생성
  2. vs code 터미널 -> git config --global user.name "깃허브 닉네임"
  3. git config --global user.email "깃허브 가입 이메일"
  4. 깃허브 페이지 코드 복사 붙혀넣기



- echo "# firstproject" >>README.md : README.md이라는 파일을 만들고 firstproject라고 내용을 입력하라는 뜻

- git init  : 현재 디렉토리를 새로운 깃 저장소로 초기화한다는 뜻. 이렇게하면 숨긴파일로 깃이라는 파일이 생김

- git add : (구동과정 : staging area라는 공간에 저장할 파일을 넣어주고 staging area를 통쨰로 저장)

     * git status : git 상태 확인 명령어
     * git add . : 현재 디렉토리에 있는 모든 파일이 올라감
        * git add 파일이름 파일이름 : 파일이름, 파일이름이 올라감
        * gitignore : 올리지 말아야할 파일 -> .gitignore파일 생성 (gitignore.io사이트 접속 django입력 복붙)

- git commit 

  - git log : git에 commit한 내용확인
  - git commit -m "commit 내용"

- branch

  - git branch -M main : master branch의 이름을 main으로 바꾼다는 뜻 (master이름을 그냥 사용하고 싶으면 안 써도 됨)
  - git branch "브랜치이름"
  - git checkout "브랜치 이름"
  - git status : 현재 위치 확인

  #### 총정리

- ##### 새로 만들때

  - git init
  - git add
  - git commit -m "message"
  - git remote add [remote 이름] [repository 주소]
  - git push [remote 이름] [branch 이름]

- ##### 코드 수정

  - git add
  - git commit -m "message"
  - git push [remote 이름] [branch 이름]



### 4. Django와 데이터베이스

- 변수나 함수에 f12를 누르면 선언부로 이동이 가능하다.
- 장고와 데이터베이스
  - ORM : Object Relation Mapping
  - **models.py**
  - python 객체지향 
  - class



### 5. Model 실습

- 실습

  1. 앱생성 : python mange.py startapp [앱이름]
  2. settings.py -> 앱이 하나 생성됐다고 등록
  3. 앱에서 models.py -> database 칼럼 작성 class를 통해서
  4. 작성이 완료되면 python manage.py **makemigrations** -> 테이블을 이렇게 만들거라고 migrations라는 폴더에 저장
  5. python mange.py **migrate** -> migrations 폴더를 뒤져서 변경사항들을 db.sqlite에 적용을 시킴
  6. admin 처음 들어갈 때 superuser계정 생성해야함
  7. 터미널 들어가서 python manage.py createsuperuser -> 계정 생성
  8. admin.py -> models.py에 앱을 등록했다고 알려줘야함 
     - from .models import Blog
     - admin.site.register(Blog)

  

- **makemigrations** : 앱 내의 migration 폴더를 만들어서 models.py의 변경사항 저장
- **migrate** : migration폴더를 실행시켜 데이터베이스에 적용
- 상속받은 class Blog(models.Model) -> Model에 id는 이미 상속되어 있음

- runserver한 다음에 /**admin**으로 들어가면 database를 볼 수 있음



### 6. CRUD-Read

- 실습
  1. templates에 html하나 생성
  2. views.py -> 함수하나 생성

- CRUD (데이터베이스를 crud한다.)
  - create 생성하다
  - read 읽다
  - update 수정하다
  - delete 삭제하다
- views.py에 함수가 하나 생성될 때 무조건 urls.py에 path가 하나 추가된다고 생각하기!!!

- 주석처리 단축키 : ctrl + ? 

 

- **path-converter** : path('<str:id>',detail,name="detail")



### 7. CRUD-Create

- CRUD
  - new: new.html 보여줌
  - create: 데이터베이스에 저장



### 8. CRUD-Update

- CRUD
  - edit: edit.html 보여줌
  - update: 데이터베이스에 적용
  - **수정할 데이터의 id값을 받아야함**
  
  

### 9. CRUD-Delete

### 10. Template 상속

- 불필요한 코드를 사용하지 않기 위한! 내가 궁금했던 것 개꿀~!
- 중복되는 코드를 base.html을 사용해 정리한다.
- urls.py도 상속가능. 앱별로 상속



### 11. Static

- 정적 파일 vs 동적파일
  - 정적파일 : 미리 서버에 저장되어 있는 파일, 서버에 저장되 그대로를 서비스해주는 파일
    - Static : 개발자가 서버를 개발할 때 미리 넣어놓은 정적파일 (Img, js, css)
    - media : 사용자가 업로드 할 수 있는 파일
  - 동적파일 : 서버의 데이터들이 어느정도 가공된다음 보여지는 파일 (상황에 따라 달라질 수 있음)

  

  python manage.py collectstatic -> static 파일들을 한곳에 저장

  

### 12. Media

![image-20210628224809101](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20210628224809101.png)

![image-20210628224834120](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20210628224834120.png)

웹 통신 방식은 url이다



### 13. Form

- Form : 입력공간

- forms.py



### 14. User 확장과 인증

- 사용자에 따라 페이지에 보여지는게 다름 
- 장고에서 제공해주는  auth
- Authentication : 인증
- ![image-20210628225324218](C:\Users\82108\AppData\Roaming\Typora\typora-user-images\image-20210628225324218.png)
- 클라이언트의 인증 관리 함수 : authenticate, login, logout



### 15. Paginator

- paginator : 블로그 객체를 잘라서 보내줌

- 페이지 관련 정보도 있음 (/?**page = paginator.어떤페이지**)




### 16. 배포 사전준비

- **환경변수?**

  시스템에 저장되어 있는 변수

  보통 비밀키 등 유출되면 안되는 정보

  또는 환경에 차이를 둘 때 사용 (테스트/프로덕션 구별 등)

  os.environ 에서 dict 형식으로 불러올 수 있음

  os.environ.get('변수명','기본값') 으로 사용

- **requirements?**

  내 파이썬 (장고) 앱을 실행하기 위해 우선 설치되어야 하는 패키지들

  Django, Pillow 등

  패키지명 == 버전으로 저장

  보통 requirements.txt 파일에 저장

  pip freeze 명령어는 해당 환경에 설치된 모든 패키지를 보여줌

  /> 는 프로그램의 출력을 파일에 저장한다는 뜻

  pip freeze > requirements.txt 로 생성

- **IAM ?**

  Identity and Access Management 의 줄임말

  IAM에서 계정을 만든 후 해당 계정 로그인 정보 (엑세스 키 $ 시크릿 키)를 이용하여 AWS의 API 활용

  보안을 위해 권한을 최대한 보수적으로 잡음

- **S3?**

  Simple Storage Service의 줄임말

  AWS에서 제공하는 구글드라이브 정도로 생각할 수 있음

  최초 용량 지정 없이 사용한 만큼만 과금되므로 용량 예측 필요 X

  여러 서버에서 동시에 접속 가능 (부하 분산 유리)

 

### 17. Heroku 배포하기

1.  Heroku 회원가입

2.  Heroku CLI 설치

3. 환경 변수 적요

   1. Debug 는 아래 값 사용
      1. DEBUG = ( os.environ.get('DEBUG',  'True') != 'False' )

4.  .gitignore 파일 적용

   1. gitignore.io 에서 Django 선택 후 '생성' 클릭
   2. 페이지에 나온 텍스트를 모두 복사후 .gitignore 파일로 저장

5. Heroku 용 파일 작성

   1. Procfile 이라는 파일을 만들어 아래 내용 작성
      1. web: gunicorn 프로젝트명.wsgi --log-file-
   2. runtime.txt 파일에 아래 내용 작성
      1. python-3. 9. 1

6. 필요한 Dependency 설치

   1. pip install gunicorn whitenoise dj-database-url psycopg2-binary

7. settings.py 수정

   1. Whitenoise 설치

      1. MIDDLEWARE 에서 제일 SecurityMiddelware 바로 아래 내용 추가
         1. 'whitenoise.middleware.WhiteNoiseMiddleware' ,

   2. ALLOWED_HOSTS 수정

      1. ALLOWED_HOSTS = [] 를 ALLOWED_HOSTS = [' * '] 로 수정

   3. DB 관련 코드 수정

      1. settings.py 제일 밑에 아래 내용 추가

         ```
         import dj_database_url
         
         db_from_env = dj_database_url.config(conn_max_age=500)
         
         DATABASES['default'].update(db_from_env)
         ```

1. requirements. txt 생성

   1. pip freeze > requirements.txt

2. git에 수정된 파일들 추가

   1. git add -A
   2. git commit -m "add files for deploying to heroku"

3. Heroku 관련 명령어들 실행

   1. heroku login
   2. heroku create
   3. git push heroku main
   4. heroku run python manage.py migrate
   5. heroku run python manage.py createsuperuser
   6. heroku open

4. Heroku 에서 환경 변수 설정

   1. [https://dashboard.heroku.com](https://dashboard.heroku.com/) 에서 앱 선택
   2. Settings
   3. Config Vars > Reveal Config Vars
   4. KEY VALUE 값에 입력후 저장

   

### 18. Ubuntu 배포하기

 https://console.aws.amazon.com/

 

### 19. Docker란?

https://www.yalco.kr/08_docker/

​	
