# border

CSS `border` 속성을 사용하면 요소 테두리의 스타일, 너비 및 색상을 지정할 수 있습니다.

## border-style

이 `border-style` 속성은 어떤 종류의 테두리를 표시할지 지정합니다.

허용되는 값은 다음과 같습니다.

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
<p style="border-style: dotted;">dotted</p>
<p style="border-style: dashed;">dashed</p>
<p style="border-style: solid;">solid</p>
<p style="border-style: double;">double</p>
<p style="border-style: groove;">groove.</p>
<p style="border-style: ridge;">ridge</p>
<p style="border-style: inset;">inset</p>
<p style="border-style: outset;">outset</p>
<p style="border-style: none;">none</p>
<p style="border-style: hidden;">hidden</p>
<p style="border-style: dotted dashed solid double;">mixed</p>
```

<p style="border-style: dotted;">dotted</p>
<p style="border-style: dashed;">dashed</p>
<p style="border-style: solid;">solid</p>
<p style="border-style: double;">double</p>
<p style="border-style: groove;">groove.</p>
<p style="border-style: ridge;">ridge</p>
<p style="border-style: inset;">inset</p>
<p style="border-style: outset;">outset</p>
<p style="border-style: none;">none</p>
<p style="border-style: hidden;">hidden</p>
<p style="border-style: dotted dashed solid double;">mixed</p>


## bower-width 

`border-width` 속성은 네 개의 테두리의 너비를 지정합니다.

너비는 특정 크기(px, pt, cm, em 등) 또는 미리 정의된 세가지 값 중 하나인 thin, medium, thick 중 하나를 사용하여 설정할 수 있습니다.

`border-width` 속성은 1~4 개의 값에서(위쪽, 오른쪽, 아래쪽, 왼쪽 순서) 지정할  수 있습니다.

```css
p.one {
  border-style: solid;
  border-width: 5px;
}

p.two {
  border-style: solid;
  border-width: medium;
}

p.three {
  border-style: solid;
  border-width: 2px 10px 4px 20px;
}
```

## border-color

`border-color` 속성은 네 개의 테두리 색상을 설정하는데 사용됩니다.

색상은 다음과 같이 설정할 수 있습니다.

- name : "red" 와 같은 색상 이름을 지정하십시오.
- 16진수 : "#ff0000"과 같은 16 진수 값 지정
- RGB : RGB값을 지정합니다(예 : "rgb(255,0,0)")
- transparent : 투명

`border-color` 속성은 1~4 개의 값에서(위쪽, 오른쪽, 아래쪽, 왼쪽 순서) 지정할  수 있습니다.

만약 `border-color` 가 설정되지 않으면 요소의 색상을 상속받습니다.

```css
p.one {
  border-style: solid;
  border-color: red;
}

p.two {
  border-style: solid;
  border-color: green;
}

p.three {
  border-style: solid;
  border-color: red green blue yellow;
}
```


## border 개별 적용

border 는 4개의 면을 각기 다른스타일로 적용할 수 있습니다.

```css
p {
    border-top-style: dotted;
    border-right-style: solid;
    border-bottom-style: dotted;
    border-left-style: solid;
}
```

## border 단축속성

`border-width`, `border-style(필수)`, `border-color` 의 속성을 한번에 지정할 수도 있습니다.

```css
p {
    border: 5px solid red;
}
```

## 모든 CSS border 속성

속성 | 설명 
---------- | -----------
border | 하나의 선언에 모든 ​​테두리 속성을 설정합니다.
border-bottom | 하나의 선언에 모든 ​​아래쪽 테두리 속성을 설정합니다.
border-bottom-color | 아래쪽 테두리의 색을 설정합니다.
border-bottom-style | 아래쪽 테두리의 스타일을 설정합니다.
border-bottom-width | 아래쪽 테두리의 너비를 설정합니다.
border-color | 네 가지 테두리의 색상을 설정합니다.
border-left | 하나의 선언에 모든 ​​왼쪽 테두리 속성을 설정합니다.
border-left-color | 왼쪽 테두리의 색상을 설정합니다.
border-left-style | 왼쪽 테두리의 스타일을 설정합니다.
border-left-width | 왼쪽 테두리의 너비를 설정합니다.
border-radius | 둥근 모서리의 반경을 설정합니다.
border-right | 하나의 선언에 모든 ​​오른쪽 테두리 속성을 설정합니다.
border-right-color | 오른쪽 테두리의 색상을 설정합니다.
border-right-style | 오른쪽 테두리의 스타일을 설정합니다.
border-right-width | 오른쪽 테두리의 너비를 설정합니다.
border-style | 네 개의 테두리의 스타일을 설정합니다.
border-top | 하나의 선언에 모든 ​​상단 테두리 속성을 설정합니다.
border-top-color | 상단 테두리의 색상을 설정합니다.
border-top-style | 위쪽 테두리의 스타일을 설정합니다.
border-top-width | 위쪽 테두리의 너비를 설정합니다.
border-width | 네 개의 테두리의 너비를 설정합니다.

