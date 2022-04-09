HTML이란 무엇인가?
==================
## 0. HTML의 역사
[팀 버너스 리](https://ko.wikipedia.org/wiki/팀_버너스리)가 HTML의 원형인 인콰이어를 제안하였는데,
인터넷의 기반을 닦은 여러 공로로 웹의 아버지라고 불리는 인물 중 하나입니다.
현재 그는 차세대 웹 기술인 시맨틱 웹 기술의 표준화에 힘쏟고 있습니다.

_여담으로, http://~~~ 에서 //는 없어도 잘 돌아가는 것을 볼 수 있는데, 단순히 멋있어보여서 넣었다고 합니다..._

이 글의 내용들은 학교와 동아리, 그리고 [생활코딩](https://opentutorials.org/course/3084)의 내용들을 기반으로 제작되었습니다.   
초보자에게 좋은 강의이니 가셔서 공부해보는 걸 추천합니다.

## 1. HTML 기본 용어
### 1.1 기본 틀과 태그
다음은 HTML의 기본적인 형식이다.

`<!DOCTYPE html>` : Document type declaration(=문서 형식 선언), HTML파일일 경우 반드시 첫 줄에 넣어야 합니다.   
`<html>` : 모든 HTML 페이지의 기본 요소로, 모든 태그는 이 HTML 태그 내부에 작성한다.   
`<head>` : body 태그에 필요한 스타일시트와 자바스크립트를 제공한다.   
`<title>` : 웹 브라우저에 표시하는 제목을 지정한다.   
`<style>` : 스타일시트이다.   
`<body>` : 사용자에게 실제로 보이는 부분을 작성하는 곳이다.   

```html
<!DOCTYPE html>
<html>
    <head>
        <title>Hello Html5</title>
        <style>
            h1 {
                color: gold;
                background: black;
            }
        </style>
    </head>
    <body>
        <h1>Hello world!</h1>
    </body>
</html>
```
이런 식으로 작성할 수 있다.
### 1.2 기본 태그

`<h1>`의 h는 헤더의 약자로 제목 글자 태그이다.
```html
<h1>Hello world</h1>
<h2>Hello world</h2>
<h3>Hello world</h3>
<h4>Hello world</h4>
<h5>Hello world</h5>
<h6>Hello world</h6>
```
이들은 각각

<h1>Hello world</h1>
<h2>Hello world</h2>
<h3>Hello world</h3>
<h4>Hello world</h4>
<h5>Hello world</h5>
<h6>Hello world</h6>
에 해당합니다(숫자와 크기는 반비례 관계)   
<hr>

글들을 강조하고자 할때에는   
`<strong>`~~강하다!~~   
그 중에서도 강조(=밑줄)하고자 하는 것에는   
`<u>`~~여기 밑줄~~   
이러한 태그들을 사용할 수 있습니다.

위에 나온 여러 태그들을 통해 HTML을 구성할 수 있습니다.

` <p> 본문 문단 생성 </p> `   
<p>본문 문단 생성 </p>

` <br> `   
줄바꿈   
<br>

` <hr> `   
수평 줄 생성   
<hr>

`<br>`과 `<hr>`은 닫지 않는 것을 볼 수 있는데, 태그 내부에 넣을 속성이 없기 때문입니다. [[참조]](https://ofcourse.kr/html-course/%ED%83%9C%EA%B7%B8)

### 1.3 속성

태그의 심화된 문법입니다.

`<img>` 태그에 source의 줄임말인 `src`를 넣어서   
`<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png">`와 같이 입력하면   
<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png">   
이미지가 나타나는 것을 볼 수 있습니다.

이제 위의 이미지의 크기를 줄여봅시다. width 속성을 이용해서 숫자나 %를 사용하면 원하는 크기로 조정할 수 있습니다.   
`<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png" width="60%">`   
<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png" width="60%">

`<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png" width="400px">`   
<img src="https://s3-ap-northeast-2.amazonaws.com/opentutorials-user-file/module/3135/7648.png" width="400px">   
px는 생략할 수 있다