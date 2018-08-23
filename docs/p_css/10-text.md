# text

`color` 속성은 텍스트의 색을 설정하는데 사용됩니다. 색상은 다음과 같이 지정됩니다.

- 색상 이름 : 예: "red"
- HEX값 : 예: "#ff0000"
- RGB값 : 예: "rgb(255,0,0)"

가능한 색상 값의 전체 목록을 보려면 [CSS 색상값](https://www.w3schools.com/cssref/css_colors_legal.asp) 을 보십시오.

```css
body {
  color: blue;
}
```

## text-align

text-align속성은 텍스트의 가로 맞춤을 설정하는 데 사용됩니다.

텍스트는 왼쪽 또는 오른쪽 정렬, 가운데 맞춤 또는 양쪽 맞춤이 가능합니다.

```css
h1 {
    text-align: center;
}

h2 {
    text-align: left;
}
```


## text-decoration

`text-decoration` 속성은 텍스트에 장식을 설정하거나 제거하는데 사용됩니다.

이 값 text-decoration: none;은 종종 링크에서 밑줄을 제거하는데 사용됩니다.

```css
a {
    text-decoration: none;
}
h1 {
    text-decoration: overline;
}
h2 {
    text-decoration: line-through;
}
h3 {
    text-decoration: underline;
}
```

## text-transform

`text-transform` 속성은 텍스트에서 대문자와 소문자를 지정하는데 사용됩니다.

모든 것을 대문자 또는 소문자로 바꾸거나 각 단어의 첫 글자를 대문자로 사용할 수 있습니다.

```css
p.uppercase {
    text-transform: uppercase;
}

p.lowercase {
    text-transform: lowercase;
}

p.capitalize {
    text-transform: capitalize;
}
```

## text-indent

`text-indent` 속성은 텍스트의 첫번째줄에 들여 쓰기를 지정하는데 사용됩니다.

```css
p {
    text-indent: 50px;
}
```

## letter-spacing

`letter-spacing` 속성은 텍스트의 문자 사이 간격을 지정하는데 사용됩니다.

```css
h1 {
    letter-spacing: 3px;
}
h2 {
    letter-spacing: -3px;
}
```

## line-height

`line-height` 속성은 줄 사이의 간격을 지정하는데 사용됩니다.

```css
.small {
    line-height: 0.8;
}
```


## direction

`direction` 속성은 요소의 텍스트 방향을 변경하는데 사용됩니다.


```css
p {
    direction: rtl;
}
```

## word-spacing

`word-spacing` 속성은 텍스트의 단어 사이의 공백을 지정하는데 사용됩니다.

```css
h1 {
    word-spacing: 10px;
}
```



속성 | 설명 
---------- | -----------
color | 텍스트의 색을 설정합니다.
direction | 텍스트 방향 / 쓰기 방향을 지정합니다.
letter-spacing | 텍스트의 문자 사이의 간격을 늘리거나 줄입니다.
line-height | 줄 높이를 설정합니다.
text-align | 텍스트의 가로 정렬을 지정합니다.
text-decoration | 장식을 텍스트에 추가하도록 지정합니다.
text-indent | 텍스트 블록의 첫번째 줄의 들여 쓰기를 지정합니다.
text-transform | 텍스트의 대소문자를 제어합니다.
text-overflow | 표시되지 않은 오버플로우 된 콘텐츠를 사용자에게 전달하는 방법을 지정합니다.
unicode-bidi | direction 속성과 함께 사용하여 동일한 문서에서 여러 언어를 지원하도록 텍스트를 재정의해야 하는지 여부를 설정하거나 반환합니다.
vertical-align | 요소의 수직 정렬을 설정합니다.
white-space | 요소 내부의 공백을 처리하는 방법을 지정합니다.
word-spacing | 텍스트에서 단어 사이의 간격을 늘리거나 줄입니다.





