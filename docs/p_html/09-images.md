# Images

HTML 에서 이미지를 표현하려면 `<img>` 태그를 사용합니다.

!!! tip
    `<img>` 태그는 닫기태그가 없습니다.

`src` 속성은 이미지의 주소을 지정합니다.  
`alt` 속성은 대체텍스트를 지정합니다. 대체텍스트는 이미지의 설명입니다. 브라우져가 이미지를 찾을수 없으면 alt 속성값이 표시됩니다.

!!! tip
    alt 속성은 필수입니다.

코드예:
```html
<img src="https://developers.google.com/identity/images/g-logo.png" alt="">
```

보여지는예:
<img src="https://developers.google.com/identity/images/g-logo.png" alt="">


# Image Maps

`<map>` 태그를 사용하여 이미지 맵을 정의할수 있습니다. 이미지 맵은 클릭 가능한 영역이 있는 이미지입니다.  
`<area>` 요소를 사용하여 이미지 맵에서 클릭 가능한 영역을 정의합니다.  
`<img>`의 요소 `usemap` 속성을 사용하여 이미지맵을 가리킵니다.  

코드예:
```html
<img src="https://www.w3schools.com/html/workplace.jpg" alt="Workplace" usemap="#workmap">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="https://www.w3schools.com/html/computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="https://www.w3schools.com/html/phone.htm">
  <area shape="circle" coords="337,300,44" alt="Coffee" href="https://www.w3schools.com/html/coffee.htm">
</map>
```

아래 이미지에서 컴퓨터, 전화 또는 커피잔을 클릭하십시오.
보여지는 예:

<img src="https://www.w3schools.com/html/workplace.jpg" alt="Workplace" usemap="#workmap">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="https://www.w3schools.com/html/computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="https://www.w3schools.com/html/phone.htm">
  <area shape="circle" coords="337,300,44" alt="Coffee" href="https://www.w3schools.com/html/coffee.htm">
</map>
