## html 이란?
html은 웹페이지를 만들기위한 표준 마크업 언어입니다.

- HTML 은 `Hyper Text Markup Language` 입니다.
- HTML 은 마크업을 사용하여 웹페이지의 구조를 설명합니다.
- HTML 요소는 html 페이지의 구성요소입니다.
- HTML 요소는 태그로 표현됩니다.
- 브라우져는 HTML 태그를 표시하지 않지만 이를 사용하여 페이지의 내용을 렌더링합니다.

## html 의 기본구조

```html
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>해딩</h1>
<p>단락</p>

</body>
</html>
```

## 에디터

메모장, 텍스트 편집기 등을 사용하여 html 을 작성합니다.  
전문적인 편집기를 사용하는데 주로 editplus, notepad++, sublimetext, atom, visual studio code 등을 이용합니다.  
확장자가 `.html` 로 끝나는 문서가 html 입니다.


## HTML 문서
모든 html 문서는 `<! DOCTYPE html>` 과 같은 문서 유형 선언으로 시작해야 합니다.  
HTML 문서 자체는 `<html>` 로 시작하고 `</html>`로 끝납니다.  
HTML 문서의 보이는 부분은 `<body>` 와 `</body>` 사이에 있습니다.

문서형 정의(DTD:Document Type Definition)은 HTML5, XHTML, HTML의 세가지 문서 유형이 존재하며, 기술한 유형에 따라 마크업 문서의 요소와 속성등을 처리하는 기준이 되며 유효성 검사에 이용된다.

## XHTML

- XHTML 문서는 올바르게 중첩 되어야 합니다.
- XHTML 문서는 항상 닫혀 있어야 합니다.
- XHTML 문서는 소문자여야 합니다.
- XHTML 문서에는 하나의 루트 요소가 있어야 합니다.
- 속성 이름은 소문자여야 합니다.
- 속성 값은 따옴표로 묶어야 합니다.
- 속성 최소화는 금지되어 있습니다.

## 문서타입 선언

- HTML 4.01 DOCTYPE 선언
strict DTD, Transitional DTD, Frameset DTD

```html
<!-- strict DTD -->
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
```

- XHTML 1.0 DOCTYPE 선언
strict DTD, Transitional DTD, Frameset DTD

```html
<!-- Transitional DTD -->
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1-transitional.dtd">
```

- HTML5 DOCTYPE 선언

```html
<!DOCTYPE html>
```

## HTML 버젼

버젼 | 연도
----|-----
html | 1991
html 2.0 | 1995
html 3.2 | 1997
html 4.01 | 1999
xhtml | 2000
html5 | 2014

## HTML 요소

HTML 요소는 시작 태그와 종료 태그로 구성됩니다.

`<tagname>` 콘텐츠는 여기에 있습니다 ... `</tagname>`


> 내용이 없는 HTML 요소를 빈태그 라고합니다. 빈태그에는 `<br>` 태그(줄 바꿈을 나타냄)와 같은 닫기 태그가 없습니다.


## 소문자 태그 사용
HTML 태그는 대소 문자를 구분하지 않습니다. `<P>`는 `<p>`와 같습니다.  
HTML5 표준은 소문자 태그를 필요로하지 않지만 W3C 는 HTML에서 소문자를 권장하고 XHTML과 같이 더 엄격한 문서 유형의 경우 소문자를 요구 합니다.


## HTML 속성
모든 HTML 요소는 속성을 가질 수 있습니다.
속성은 요소에 대한 추가 정보를 제공합니다.
속성은 항상 시작태그에 지정됩니다 .
속성은 일반적으로 다음과 같이 이름/값 쌍으로 옵니다. `name="value"`


