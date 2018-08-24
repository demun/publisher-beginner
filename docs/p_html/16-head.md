# <head> 요소

`<head>` 요소는 메타데이터의 컨테이너입니다. HTML 메타데이터는 HTML 문서에 대한 데이터입니다. 메타데이터는 화면에 표시되지 않습니다.  
메타데이터는 일반적으로 문서 제목, 문자 세트, 스타일, 링크, 스크립트 및 기타 메타 정보를 정의합니다.

`<head>` 요소는 `<html>` 태그와 `<body>` 태그 사이에 배치됩니다.

예:

```html
<!DOCTYPE html>
<html>
<head>
  <title>문서제목</title>
  <meta charset="UTF-8">
  ...
</head>
<body>
...
</body>
</html>
```

## `<title>` 
`<title>` 요소는 문서의 제목을 정의합니다.

```html
<!DOCTYPE html>
<html>
<head>
  <title>문서제목</title>
</head>
<body>
...
</body>
</html>
```


## `<style>` 
`<style>`요소는 하나의 HTML 페이지에 대한 스타일 정보를 정의하는데 사용됩니다.

```html
<style>
  body {background-color: powderblue;}
  h1 {color: red;}
  p {color: blue;}
</style>
```


## `<link>` 
`<link>` 요소는 외부 스타일시트에 연결하는데 사용됩니다.

```html
<link rel="stylesheet" href="mystyle.css">
```



## `<meta>`
`<meta>` 요소는 페이지 설명, 키워드, 제작자 및 다른 메타 데이터를 사용하는 문자 세트를 지정하는데 사용된다.  
메타데이터는 브라우저(내용 표시 방법), 검색 엔진(키워드) 및 기타 웹 서비스에서 사용됩니다.


```html
<head>
  <meta charset="UTF-8">
  <meta name="description" content="사이트의 설명">
  <meta name="keywords" content="키워드">
  <meta name="author" content="제작자">
</head>
```



## `<script>`

`<script>` 요소는 클라이언트 측 JavaScript를 정의하는데 사용됩니다.

```html
<script>
function myFunction {
    document.getElementById("demo").innerHTML = "Hello JavaScript!";
}
</script>
```




## `<base>`
`<base>` 요소는 페이지의 모든 상대 URL에 대한 기본 URL과 기본 대상을 지정합니다.

```html
<base href="https://www.w3schools.com/images/" target="_blank">
```

## file paths
