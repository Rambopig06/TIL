# JS 를 활용한 웹페이지 개발 1

## html 의 시멘틱 태그란?

`semantic : 의미있는 , 의미론 적인`<br/>

html 을 사용하여 웹 페이지를 제작할 때<br/>
'시멘틱 태그'라는걸 사용하여 기초를 가진다.<br/>
<br/>
인간의 신체를 예시로 들어봤을 때,<br/>
머리 , 어깨 , 무릎 , 발 등으로 고유한 신체 명칭이 있다.<br/>
웹 사이트 제작시에도 대표적으로 위에서부터<br/>
`header : 머리`<br/>
`nav : 내비게이션 바`<br/>
`section : 메인 내용`<br/>
`footer : 푸터`<br/>
등으로 나뉜다.<br/>
<br/>
div 같은 명령어에 class나 id 옵션을 사용하여<br/>
각 항목의 역할과 이름을 부여하기도 하지만<br/>
사이트를 제작할 때 위와 같은 기초적인 부분까지<br/>
div 로 통일 시키고 class 등으로 이름을 붙이면<br/>
<br/>
너무 너무 복잡하고 드러운 코드가 만들어진다.<br/>
<br/>
이러한걸 해결하기 위해 html5 기준 시멘틱 태그는<br/>
`header` `nav` `section` `footer` `article` `aside`<br/>
`details` `figcaption` `figure` `main` `mark` `time` `summary`<br/> 
가 있다.<br/>
<br/>

이제 이 시멘틱 태그와 JS 를 혼합하여<br/>
On / Off 스위치를 만들어 보겠다.<br/>
<br/>

## HTML 시멘틱 태그를 활용해 웹페이지의 뼈대 만들기

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>토글 스위치</title>
</head>
<body>
     
</body>
</html>
```
VS code 를 열고 html 확장자 파일 까지 만든다음,<br/>
! 를 입력후 \<tab> 을 누르면<br/>
<br/>
이렇게 기본적인 양식이 완성된다.<br/>
웹 페이지의 뼈대는 이 코드 속<br/>
\<body>\</body> 내에서 작업한다.<br/>
<br/>

```
<body>
     <header></header>
     <nav></nav>
     <section></section>
     <footer></footer>
</body>
```
아주 기초적인 뼈대 구성이다.<br/>
뼈대를 제작했으니 이제 살을 붙이고 네일을 칠해보자.<br/>
<br/>

## CSS 로 HTML 코드에 살 붙이기
`CSS : Cascading Style Sheet`<br/>
웹 페이지의 레이아웃과 디자인을 제작하는 언어이다.<br/>
HTML과 단짝으로 같이 다니는 언어일 수 밖에 없다.<br/>
<br/>
이제 CSS 확장자 파일과 HTML 파일을 연동하기위한<br/>
작업을 해보겠다.<br/>
<br/>

(CSS 연결)

html 코드에서 body 태그 밖에 link 태그를 입력 후<br/>
\<tab> 을 눌러 완성시키면<br/>

`<link rel="stylesheet" href="">`<br/>
이런 코드가 생성된다.<br/>
<br/>
rel 은 relation, 즉 관계를 뜻하는데<br/>
하이퍼링크를 뜻하는 href 에 적을 파일과<br/>
무슨 관계인건지를 묻는 코드이다.<br/>
<br/>
style.css 코드는 index.html 코드의 스타일시트를 담당하므로<br/>
rel 옆에 stylesheet 를 입력하고,<br/>
href 옆에는 style.css 의 경로를 입력한다.<br/>
<br/>


<br/>
