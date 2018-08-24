# introduction

자바스크립트는 웹프로그래밍 언어입니다.

HTML 은 웹페이지의 내용을 정의하고, CSS 는 스타일을 정의하고, JAVASCRIPT 는 동작을 정의합니다.

## 위치

HTML 에서는 `<scirpt>`태그와 `</script>` 태그사이에 JAVASCIRPT 코드를 삽입합니다.

```js
<script>
  document.getElementById("demo").innerHTML = "My First JavaScript";
</script>
```

JAVASCIRPT 는 `<head>` 태그사이 또는 `<body>` 태그사이 어디에 삽입해도 됩니다.

#### 외부 자바스크립트

외부 자바스크립트 파일을 포함할수 있습니다.

외부 자바스크립트 파일은 `.js` 확장명을 가지며, `<script>` 태그의 `src` 속성으로 추가합니다.

```js
<script src="script.js" />
```

경로는 절대경로, 상대경로 모두 사용가능합니다.

```javascript
// 절대경로
<script src="https://www.w3schools.com/js/script.js"></script>

// 상대경로
<script src="/js/script.js" />
```

외부 자바스크립트를 사용하면 HTML 과 자바스크립트 코드를 분리해서 읽기 쉽고, 유지관리하기 좋습니다.

## 출력하기

자바스크립트는 다양한 방법으로 데이터를 표시할 수 있습니다.

- `innerHTML` 를 사용하여 HTML 에 표시하는 방법
- `document.write()` 를 사용하여 HTML 에 표시하는 방법
- `windows.alert()` 를 사용하여 HTML 에 표시하는 방법
- `console.log()` 를 사용하여 HTML 에 표시하는 방법

#### `innerHTML`

HTML 요소에 접근하기 위해 `document.getElement.Id(id)` 매서드를 사용할 수 있습니다. `id` 속성은 HTML 요소를 정의합니다.

```javascript
<!DOCTYPE html>
<html>
<body>

<h1>My First Web Page</h1>

<p id="demo"></p>

<script>
document.getElementById("demo").innerHTML = 5 + 6;
</script>

</body>
</html>
```

<a href="/ex/innerHTML.html" target="_blank">예제파일 보기</a>

#### `document.write()`

HTML 문서가 완전히 로드된 후 `document.write()`를 사용하면 기존 HTML 이 모두 삭제됩니다.

```javascript
<!DOCTYPE html>
<html>
<body>

<h1>My First Web Page</h1>
<p>My first paragraph.</p>

<button
 type="button" onclick="document.write(5 + 6)">Try it</button>

</body>
</html>
```

<a href="/ex/document.write.html" target="_blank">예제파일 보기</a>

#### `windows.alert()`

`alert`을 사용하여 표시하는 방법

```javascript
<!DOCTYPE html>
<html>
<body>

<h1>My First Web Page</h1>
<p>My first paragraph.</p>

<script>
window.alert(5 + 6);
</script>

</body>
</html>
```

<a href="/ex/alert.html" target="_blank">예제파일 보기</a>

<!-- [예제파일](/ex/alert.html) -->

#### `console.log()`

디버깅을 위해 `console.log()` 메서드를 사용하여 데이터를 표시할 수 있습니다.

```javascript
<!DOCTYPE html>
<html>
<body>

<script>
console.log(5 + 6);
</script>

</body>
</html>
```

<a href="/ex/console.log.html" target="_blank">예제파일 보기</a>
