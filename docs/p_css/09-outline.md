# outline

`outline` 요소를 "눈에 띄게" 만들기 위해 테두리를 제외한 요소 주위에 그려지는 선입니다.

![outline](../../img/outline.gif)

다음과 같은 속성이 있습니다.

- outline-style
- outline-color
- outline-width
- outline-offset
- outline

> outline은 테두리와 다릅니다! 테두리와는 달리, outline은 요소의 테두리 외부로 그려지며 다른 내용과 겹칠 수 있습니다. 또한 outline은 요소의 일부가 아닙니다. 요소의 전체 너비와 높이는 outline의 너비에 영향을 받지 않습니다.

## outline-style

`outline-style` 속성은 외곽선의 스타일을 지정하며 다음 값 중 하나를 가질 수 있습니다.

속성 | 설명 
---------- | -----------
dotted | 점 형태의 테두리를 정의합니다.
dashed | 점선 형태의 테두리를 정의합니다.
solid | 단선 형태의 테두리를 정의합니다.
double | 이중 단선 형태의 테두리를 정의합니다.
groove | 그루브 테두리를 정의합니다. 효과는 테두리 색 값에 따라 다릅니다.
ridge | 돌기 형태의 테두리를 정의합니다. 효과는 테두리 색 값에 따라 다릅니다.
inset | 안으로 들어간 형태의 테두리를 정의합니다. 효과는 테두리 색 값에 따라 다릅니다.
outset | 밖으로 나온 형태의 테두리를 정의합니다. 효과는 테두리 색 값에 따라 다릅니다.
none | 테두리 없음 정의
hidden | 숨겨진 테두리를 정의합니다.

```html
<p style="outline-style: dotted;">dotted</p>
<p style="outline-style: dashed;">dashed</p>
<p style="outline-style: solid;">solid</p>
<p style="outline-style: double;">double</p>
<p style="outline-style: groove;">groove.</p>
<p style="outline-style: ridge;">ridge</p>
<p style="outline-style: inset;">inset</p>
<p style="outline-style: outset;">outset</p>
<p style="outline-style: none;">none</p>
<p style="outline-style: hidden;">hidden</p>
```

<p style="outline-style: dotted;">dotted</p>
<p style="outline-style: dashed;">dashed</p>
<p style="outline-style: solid;">solid</p>
<p style="outline-style: double;">double</p>
<p style="outline-style: groove;">groove.</p>
<p style="outline-style: ridge;">ridge</p>
<p style="outline-style: inset;">inset</p>
<p style="outline-style: outset;">outset</p>
<p style="outline-style: none;">none</p>
<p style="outline-style: hidden;">hidden</p>

## outline-color

`outline-color` 속성은 외곽선의 색상을 설정하는 데 사용됩니다.

색상은 다음과 같이 설정할 수 있습니다.

- name : "red"와 같은 색상 이름을 지정할수 있습니다.
- RGB : RGB 값을 지정합니다 (예 : "rgb (255,0,0)")
- 16진수 : "#ff0000"과 같은 16 진수값 지정
- invert : 색상 반전을 수행합니다 (색상 배경에 관계없이 외곽선을 볼 수 있음)

```css
div {
    border: 1px solid black;
    outline-style: solid;
    outline-color: red;
    padding: 20px;
    background-color: gray;
}
```

<div style="border:1px solid black; outline-style:solid; outline-color:red; padding: 20px; background-color: gray;"></div>



## outline-width

`outline-width` 속성은 외곽선의 너비를 지정하며 다음값 중 하나를 가질 수 있습니다.

- thin(1px)
- medium(3px)
- thick(5px)
- 특정크기(px, pt, cm, em 등)

```css
div {
    border: 1px solid black;
    outline-style: solid;
    outline-color: red;
    outline-width: thin;
    padding: 20px;
    background-color: gray;
}
```

미리보기

<div style="border: 1px solid black; outline-style: solid; outline-color: red; outline-width: thin; padding: 20px; background-color: gray;"></div>

## 단축속성

`outline` 속성은 다음과 같은 외곽선 속성을 설정하기위한 단축속성입니다.

- outline-width
- outline-style (필수)
- outline-color

`outline` 속성은 상기 목록에서 하나, 2 또는 3의 값으로 지정된다. 값의 순서는 중요하지 않습니다.

```css
div {
  outline: 5px solid yellow;
}
```

미리보기

<div style="outline: 5px solid yellow;"></div>


## outline-offset

`outline-offset` 속성은 외곽선과 요소의 가장자리/경계 사이에 공백을 추가합니다. 요소와 그 윤곽선 사이의 공간은 투명합니다.

```css
div {
    margin: 30px;
    border: 1px solid black;
    outline: 1px solid red;
    outline-offset: 15px;
    padding: 20px;
    background: yellow;
}
```

미리보기

<div style="margin: 30px; border: 1px solid black; outline: 1px solid red; outline-offset: 15px; padding: 20px; background: yellow;"></div>


## 모든 outline 속성

속성 | 설명 
---------- | -----------
outline | outline-width, outline-style, outline-color 를 하나의 선언으로 설정하기 위한 단축속성
outline-color | 외곽선의 색상을 설정합니다.
outline-offset | 외곽선 요소의 가장자리 또는 경계 사이의 간격을 지정합니다.
outline-style | 외곽선 스타일을 설정합니다.
outline-width | 외곽선 너비를 설정합니다.


