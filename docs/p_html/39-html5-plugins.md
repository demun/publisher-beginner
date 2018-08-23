# Plugin

`<object>` 태그 또는 `<embed>` 태그를 사용하여 웹 페이지에 플러그인을 추가 할 수 있습니다. 

플러그인은 여러가지 목적으로 사용될 수 있습니다: 지도 표시, 바이러스 검사, 은행 ID 확인 등.


# `<object>`

`<object>` 요소는 모든 브라우저에서 지원됩니다.

`<object>` 요소는 HTML 문서내에 포함된 객체를 정의합니다.

웹 페이지에 플러그인 (예: Java 애플릿, PDF 판독기, Flash Player)을 내장하는데 사용됩니다.

코드예:

```html
<object width="400" height="50" data="bookmark.swf"></object>
```

`<object>` 요소를 사용하여 HTML에 HTML을 포함시킬 수도 있습니다.

```html
<object width="100%" height="500px" data="snippet.html"></object>
```



# `<embed>`
`<embed>` 요소는 모든 주요 브라우저에서 지원됩니다.

`<embed>` 요소는 HTML 문서내에 포함된 객체를 정의합니다.

웹 브라우저는 오랫동안 `<embed>` 요소를 지원했습니다. 그러나 HTML5 이전에는 HTML 사양에 포함되지 않았습니다.

코드예:

```html
<embed width="400" height="50" src="bookmark.swf">
```

!!! tip
    `<embed>` 요소에는 닫는 태그가 없습니다. 대체 텍스트를 포함 할 수 없습니다.


`<embed>` 요소를 사용하여 HTML을 HTML에 포함 할 수도 있습니다.

```html
<embed width="100%" height="500px" src="snippet.html">
```

