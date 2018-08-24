# link

링크의 스타일을 지정할 수 있습니다.

```css
a {
  color: blue;
}
```

링크의 상태에 따라 각각 스타일을 지정할 수도 있습니다.

- a:link - 방문하지 않은 링크
- a:visited - 사용자가 방문한 링크
- a:hover - 사용자가 링크에 마우스를 올릴때
- a:active - 사용자가 링크를 클릭할 때

`link,visited,hover,active` 순서로 지정해야 합니다.

```css
a:link {
    color: red;
}
a:visited {
    color: green;
}
a:hover {
    color: hotpink;
}
a:active {
    color: blue;
}
```

## text-decoration

`text-decoration` 속성은 주로 링크에서 밑줄을 제거하는 데 사용됩니다.

```css
a:link {
    text-decoration: none;
}
```


## background-color

`background-color` 속성은 링크의 배경색을 지정할 수 있습니다 :

```css
a:link {
    background-color: yellow;
}
```


