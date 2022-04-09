HTML이란 무엇인가?
==================
## HTML의 역사
[팀 버너스 리](https://ko.wikipedia.org/wiki/팀_버너스리)가 HTML의 원형인 인콰이어를 제안하였는데,
인터넷의 기반을 닦은 여러 공로로 웹의 아버지라고 불리는 인물 중 하나입니다.
현재 그는 차세대 웹 기술인 시맨틱 웹 기술의 표준화에 힘쏟고 있습니다.

_여담으로, http://~~~ 에서 //는 없어도 잘 돌아가는 것을 볼 수 있는데, 단순히 멋있어보여서 넣었다고 합니다..._

이 글의 내용들은 학교와 동아리, 그리고 [생활코딩](https://opentutorials.org/course/3084)의 내용들을 기반으로 제작되었습니다.   
초보자에게 좋은 강의이니 가셔서 공부해보는 걸 추천합니다.

## HTML의 기본 형식
다음은 HTML의 기본적인 형식이다.

`<!DOCTYPE html>` : Document type declaration(=문서 형식 선언), HTML파일일 경우 반드시 첫 줄에 넣어야 합니다.   
`<html>` : 모든 HTML 페이지의 기본 요소로, 모든 태그는 이 HTML 태그 내부에 작성합니다.   
`<head>` : body 태그에 필요한 스타일시트와 자바스크립트를 제공합니다.   
`<title>` : 웹 브라우저에 표시하는 제목을 지정합니다.   
`<style>` : 스타일시트입니다. 주로 CSS로 다룹니다.   
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
이런 식으로 작성할 수 있습니다.