# margin

`margin` 속성은 정의 된 테두리 밖의 요소 주변에 공간을 만드는 데 사용됩니다.

CSS에는 요소의 각면에 대한 여백을 지정하는 속성이 있습니다.

- margin-top
- margin-right
- margin-bottom
- margin-left

모든 margin 속성은 다음 값을 가질 수 있습니다.

속성 | 설명 
---------- | -----------
auto | 브라우저가 여백을 계산합니다.
length | px, pt, cm 등의 여백을 지정합니다.
% | 포함하는 요소의 너비에 대한 여백을 %로 지정합니다.
inherit | 부모 요소에서 여백을 상속해야 함을 지정합니다.

> 팁 : 음수 값이 허용됩니다.

```css
p {
    margin-top: 100px;
    margin-bottom: 100px;
    margin-right: 150px;
    margin-left: 80px;
}
```

## 단축속성

하나의 속성으로 사용할 수 있습니다. 순서는 `위, 오른쪽, 아래, 왼쪽` 입니다.

예제코드 | 설명 
---------- | -----------
margin: 20px | 4군데 모두 사용, margin: 20px 20px 20px 20px; 와 같음.
margin: 20px 10px | 위,아래 20px 오른쪽,왼쪽 10px
margin: 20px 10px 5px | 위 20px, 오른쪽 10px, 아래 5px, 왼쪽 10px
margin: 20px 10px 5px 1px | 위 20px, 오른쪽 10px, 아래 5px, 왼쪽 1px

## auto

`margin: auto` 속성을 설정하여 컨테이너 내에 요소를 가로로 가운데 놓을 수 있습니다.

그러면 요소가 지정된 폭을 차지하고 나머지 공간은 왼쪽과 오른쪽 여백 사이에서 균등하게 분할됩니다.

```css
div {
    width: 300px;
    height: 50px;
    margin: auto;
    border: 1px solid red;
}
```

<div style="width:300px; height:50px; margin:auto; border:1px solid red;"></div>


`margin` 은 4군데를 모두 사용함으로 위, 아래는 지정하고, 왼쪽, 오른쪽만 자동으로 하는경우도 사용할 수 있습니다.

```css
div {
    width: 300px;
    height: 50px;
    margin: 10px auto;
    border: 1px solid red;
}
```

속성 | 설명 
---------- | -----------
margin | 하나의 선언에서 margin 속성을 설정하기위한 속기 속성
margin-bottom | 요소의 아래쪽 여백을 설정합니다.
margin-left | 요소의 왼쪽 여백을 설정합니다.
margin-right | 요소의 오른쪽 여백을 설정합니다.
margin-top | 요소의 위쪽 여백을 설정합니다.

