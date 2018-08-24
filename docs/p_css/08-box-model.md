# Box Model

모든 HTML 요소는 상자로 간주 할 수 있습니다. CSS에서는 디자인과 레이아웃에 대해 "Box Model"이라는 용어를 사용합니다.

Box Model은 모든 HTML 요소를 감싸는 상자입니다. 여백, 테두리, 패딩 및 실제 내용으로 구성됩니다. 아래 이미지는 Box Model을 보여줍니다.

![박스모델](../../img/box-model.png)


미리보기

<div style="background-color:lightgray; width:300px; border:25px solid green; padding:25px; margin: 25px; color:blue;">Element Content</div>


```css
div {
    background-color: lightgrey;
    width: 300px;
    border: 25px solid green;
    padding: 25px;
    margin: 25px;
    color: blue;
}
```

요소의 전체 너비는 다음과 같이 계산되어야합니다.

총 요소 너비 = 너비 + 왼쪽 패딩 + 오른쪽 패딩 + 왼쪽 테두리 + 오른쪽 테두리 + 왼쪽 여백 + 오른쪽 여백

