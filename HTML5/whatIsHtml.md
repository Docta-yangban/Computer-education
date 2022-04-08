HTML이란 무엇인가?
==================
## 0. HTML의 역사
[팀 버너스 리](https://ko.wikipedia.org/wiki/팀_버너스리)가 HTML의 원형인 인콰이어를 제안하였다.
인터넷의 기반을 닦은 여러 공로로 웹의 아버지라고 불리는 인물 중 하나이다.
현재 그는 차세대 웹 기술인 시맨틱 웹 기술의 표준화에 힘쏟고 있다.

_여담으로, http://~~~ 에서 //는 없어도 잘 돌아가는 것을 볼 수 있는데, 단순히 멋있어보여서 넣었다고 한다..._

## 1. HTML 기본 용어
### 1.1 기본 틀
다음은 HTML의 기본적인 형식이다.

`<!DOCTYPE html>` : Document type declaration(=문서 형식 선언)   
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
에 해당한다(숫자가 커질수록 글자가 작아진다.)   
<hr>

` <p> 본문 문단 생성 </p> `   
<p> 본문 문단 생성 </p>

` <br> ` 줄바꿈   
<br>

` <hr> ` 수평 줄 생성   
<hr>