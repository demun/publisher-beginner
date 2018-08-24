# list

리스트에는 순서가 없는 목록(<ul>), 순서가 있는 목록(<ol>)들의 스타일을 지정할 수 있습니다.

## list-style-type

`list-style-type` 속성은 목록 항목의 유형을 지정합니다.

```css
ul {
  list-style-type: square;
}
```

원본

```html
<ul style="list-style-type: square;">
  <li>list</li>
  <li>list</li>
  <li>list</li>
</ul>
```

미리보기

<ul style="list-style-type: square;">
  <li>list</li>
  <li>list</li>
  <li>list</li>
</ul>

`list-style-type: none` 속성은 기호를 제거합니다.

## list-style-image

`list-style-image` 속성은 이미지를 목록의 기호로 지정합니다.

```css
ul {
    list-style-image: url('sqpurple.gif');
}
```

원본

```html
<ul style="list-style-image: url('https://www.w3schools.com/css/sqpurple.gif');">
  <li>list</li>
  <li>list</li>
  <li>list</li>
</ul>
```

미리보기

<ul style="list-style-image: url('https://www.w3schools.com/css/sqpurple.gif');">
  <li>list</li>
  <li>list</li>
  <li>list</li>
</ul>


## list-style-position

`list-style-position` 속성은 목록 항목 표식을 콘텐츠 흐름 내부 또는 외부에 표시할지 여부를 지정합니다.

```css
ul {
    list-style-position: inside;
}
```

원본

```html
<ul style="list-style-position: inside;">
  <li>inside</li>
  <li>inside</li>
  <li>inside</li>
</ul>
<ul style="list-style-position: outside;">
  <li>outside</li>
  <li>outside</li>
  <li>outside</li>
</ul>
```

미리보기

<ul style="list-style-position: inside;">
  <li>inside</li>
  <li>inside</li>
  <li>inside</li>
</ul>
<ul style="list-style-position: outside;">
  <li>outside</li>
  <li>outside</li>
  <li>outside</li>
</ul>


## 단축속성

하나의 선언에 모든 ​​목록 속성을 설정하는 데 사용됩니다.

```css
ul {
    list-style: square inside url("sqpurple.gif");
}
```

단축속성을 사용할 때 속성 값의 순서는 다음과 같습니다.

- `list-style-type` (list-style-image가 지정되면 어떤 이유로 이미지를 표시 할 수없는 경우이 속성의 값이 표시됩니다)
- `list-style-position` (목록 항목 표식을 콘텐츠 흐름 내부 또는 외부에 표시할지 여부를 지정)
list-style-image (이미지를 목록 항목 마커로 지정)

원본

```html
<ul style="list-style: square inside url('https://www.w3schools.com/css/sqpurple.gif');">
  <li>list</li>
  <li>list</li>
  <li>list</li>
</ul>
```

미리보기

<ul style="list-style: square inside url('https://www.w3schools.com/css/sqpurple.gif');">
  <li>list</li>
  <li>list</li>
  <li>list</li>
</ul>

