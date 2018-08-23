# color

css에서 색상 이름을 사용할 수 있습니다.

```css
.header {
  color: blue;
}
```

색상이름은 [140개이상](https://www.w3schools.com/colors/colors_names.asp)을 지원합니다.


## 색상값

색상값은 RGB, HEX, HSL, RGBA 및 HSLA 를 사용하여 색상을 지정할 수도 있습니다.


#### RGB

- rgb(red, green, blue)
- rgb(빨강,초록,파랑)

0~255 사이의 값을 사용할 수 있습니다.

```css
.header {
  color: rgb(120, 120, 120);
}
```

#### HEX

rr(빨강), gg(녹색), bb(파랑)는 00에서 ff 사이의 16진수값입니다.

- rrggbb

```css
.header {
  color: #ff0000;
}
```

같은 값일경우 축약해서 사용할수도 있습니다. `color: #f00`


#### HSL

- hsl(색조,채도,명도)
- hsl(hue, saturation, lightness)

색상은 0에서 360까지의 색상환에 대한 정도입니다. 0은 빨간색이고 120은 녹색이며 240은 파란색입니다.

채도는 백분율 값이고, 0%는 회색 음영을 나타내며 100%는 풀 컬러입니다.

밝기도 백분율, 0%는 검은 색, 50%는 밝거나 어두움, 100%는 흰색입니다.

```css
.header {
  color: hsl(39, 100%, 50%);
}
```


#### RGBA HSLA
RGBA 색상 값은 색상의 불투명도를 지정하는 알파 채널이있는 RGB 색상 값의 확장입니다.

RGBA 색상 값은 다음과 같이 지정됩니다.

`rgba(빨강,초록,파랑,알파)`

알파 매개 변수는 0.0(완전 투명)과 1.0(투명하지 않음) 사이의 숫자입니다.

```css
.header {
  color: rgba(255,99,71,0.8);
}
```

HSLA 색상 값은 색상의 불투명도를 지정하는 알파 채널이있는 HSL 색상 값의 확장입니다.

HSLA 색상 값은 다음과 같이 지정됩니다.

`hsla(색조,채도,밝기,알파)`

알파 매개 변수는 0.0 (완전 투명)과 1.0 (투명하지 않음) 사이의 숫자입니다.

```css
.header {
  color: hsla(9, 100%, 64%, 0.8);
}
```


