# background-color

`background-color` 속성은 요소의 배경색을 지정합니다.

```css
body {
  background-color: lightblue;
}
```

속성 | 설명 
---------- | -----------
color | 배경색을 지정합니다. [가능한 색상 목록](https://www.w3schools.com/cssref/css_colors_legal.asp)
transparent | 배경색을 투명하게 지정합니다. 이것이 기본값입니다.
initial | 이 속성을 기본값으로 설정합니다.
inherit | 부모 요소에서 이 속성을 상속받습니다.



# background-image
`background-image` 속성은 요소의 배경으로 사용할 이미지를 지정합니다.

기본적으로 이미지는 전체 요소를 포함하도록 반복됩니다.

```css
body {
  background-image: url("paper.gif");
}
```

속성 | 설명 
---------- | -----------
url('URL') | 이미지에 대한 URL입니다. 이미지를 두 개 이상 지정하려면 URL을 쉼표로 구분하면 됩니다.
none | 배경 이미지가 표시되지 않습니다. 이것이 기본값입니다.
linear-gradient() | 선형 그라디언트를 배경 이미지로 설정합니다. 최소 두가지 색상(위에서 아래로)을 정의해야합니다.
radial-gradient() | 방사형 그라디언트를 배경 이미지로 설정합니다. 최소 두가지 색상(가장자리에서 중앙까지)을 정의해야합니다.
repeating-linear-gradient() | 선형 그라디언트를 반복합니다.
repeating-radial-gradient() | 방사형 그라디언트를 반복합니다.
initial | 이 속성을 기본값으로 설정합니다.
inherit | 부모 요소에서 이 속성을 상속받습니다.

## background-repeat

`background-image` 의 반복 여부를 나타냅니다.

속성 | 설명 
---------- | -----------
repeat | 배경 이미지가 세로 및 가로로 반복됩니다. 적합하지 않으면 마지막 이미지가 잘립니다. 이것이 기본값입니다.
repeat-x | 배경 이미지가 수평으로만 반복됩니다.
repeat-y | 배경 이미지가 수직으로만 반복됩니다.
no-repeat | 배경 이미지가 반복되지 않습니다. 이미지는 한 번만 표시됩니다.
space | 배경 이미지는 클리핑 없이 가능한 한 반복됩니다. 처음과 마지막 이미지는 요소의 양쪽에 고정되며 공백은 이미지간에 균등하게 분산됩니다.
round | 배경 이미지가 반복되고 찌그러지거나 펴져 공간을 채웁니다(간격 없음).
initial | 이 속성을 기본값으로 설정합니다.
inherit | 부모 요소에서 이 속성을 상속받습니다.

```css
body {
  background-image: url("paper.gif");
  background-repeat: repeat-x;
}
```

## background-position

`background-image` 의 위치값을 나타냅니다.

`background-position: x시작점 y시작점`

```css
body {
  background-image: url("paper.gif");
  background-position: left top;
}
```

<table>
  <tr>
    <td>속성</td>
    <td>설명</td>
  </tr>
  <tr>
    <td>left top</td>
    <td rowspan="8">키워드 하나만 지정하면 다른 값은 "center" 가 됩니다.</td>
  </tr>
  <tr>
    <td>left center</td>
  </tr>
  <tr>
    <td>left bottom</td>
  </tr>
  <tr>
    <td>right top</td>
  </tr>
  <tr>
    <td>right center</td>
  </tr>
  <tr>
    <td>right bottom</td>
  </tr>
  <tr>
    <td>center top</td>
  </tr>
  <tr>
    <td>center center</td>
  </tr>
  <tr>
    <td>center bottom</td>
  </tr>
  <tr>
    <td>x% y%</td>
    <td>첫번째 값은 가로 위치이고 두번째 값은 세로입니다. 왼쪽 상단 모서리는 0% 0%입니다. 오른쪽 하단 모서리는 100% 100%입니다. 하나의 값만 지정하면 다른 값은 50%가됩니다. 기본값은 0% 0% 입니다.</td>
  </tr>
  <tr>
    <td>xpos ypos</td>
    <td>첫번째 값은 가로 위치이고 두번째 값은 세로입니다. 왼쪽 위 모서리는 0입니다. 단위는 픽셀(0px 0px) 또는 다른 CSS 단위 일 수 있습니다. 하나의 값만 지정하면 다른 값은 50%가 됩니다. %와 위치를 혼합 할 수 있습니다.</td>
  </tr>
  <tr>
    <td>initial</td>
    <td>이 속성을 기본값으로 설정합니다.</td>
  </tr>
  <tr>
    <td>inherit</td>
    <td>부모 요소에서 이 속성을 상속받습니다.</td>
  </tr>
</table>


## background-attachment

배경 이미지를 고정해야 할때(페이지의 나머지 부분과 함께 스크롤하지 않음) `background-attachment` 속성을 사용합니다.


```css
body {
  background-image: url("paper.gif");
  background-attachment: fixed;
}
```

속성값으로는 아래의 경우를 사용할 수 있습니다.

속성 | 설명 
---------- | -----------
fixed | 배경이미지가 페이지와 함께 스크롤되지 않습니다.
inherit | 부모 요소로부터 속성을 상속받습니다.
initial | 이 속성을 기본값으로 사용합니다.
local | 배경이미지가 요소의 내용과 함께 스크롤됩니다.
scroll | 배경이미지가 페이지와 함께 스크롤됩니다. 기본값입니다.


# 단축표기

`background: bg-color bg-image position/bg-size bg-repeat bg-origin bg-clip bg-attachment initial|inherit;` 를 한번에 지정할수도 있습니다.

속성 중 `bg-size` 속성인 경우 /(슬래시)를 사용합니다.

속성 | 설명 | CSS
---------- | ----------- | -------------
background-color | 사용할 배경색을 지정합니다 |	1
background-image | 사용할 배경 이미지를 하나 이상 지정합니다 | 1
background-position | 배경 이미지의 위치를 지정합니다 | 1
background-size | 배경 이미지의 크기를 지정합니다 | 3
background-repeat | 배경 이미지를 반복하는 방법을 지정합니다 | 1
background-origin | 배경 이미지의 위치 지정 영역을 지정합니다. | 3
background-clip | 배경 이미지의 그림 영역 지정 | 3
background-attachment | 배경 이미지가 고정되어 있는지 또는 나머지 페이지와 함께 스크롤되는지를 지정합니다 | 1
initial | 이 속성을 기본값으로 설정합니다. | 3
inherit | 부모 요소에서 이 속성을 상속받습니다 | 2



