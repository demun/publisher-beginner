# fonts

CSS 글꼴 속성은 글꼴 모음, 굵기, 크기 및 텍스트 스타일을 정의합니다.


Serif 와 Sans-serif 글꼴의 차이점

![serif](../../img/serif.gif)


## font-family

CSS에는 두 가지 유형의 font family 이름이 있습니다.

- generic family - 비슷한 모양을 가진 글꼴 패밀리 그룹(예 : "Serif" 또는 "Monospace")
- font family - 특정 글꼴 모음(예: "Times New Roman" 또는 "Arial")


텍스트의 글꼴 모음은 `font-family` 속성으로 설정됩니다 .

`font-family` 속성은 대체할수있는 여러 글꼴 이름을 포함해야합니다. 브라우저가 첫 번째 글꼴을 지원하지 않으면 다음 글꼴을 시도하는 식으로 진행됩니다.

다른 글꼴을 사용할 수 없는 경우 브라우저에서 일반 글꼴로 비슷한 글꼴을 선택하도록 원하는 글꼴로 시작하고 일반 글꼴로 끝냅니다.

참고 : 글꼴 패밀리의 이름이 두 단어 이상인 경우 "Times New Roman"과 같이 따옴표로 묶어야합니다.

하나 이상의 글꼴 군이 쉼표로 구분 된 목록으로 지정됩니다.

```css
p {
    font-family: "Times New Roman", Times, serif;
}
```

일반적으로 사용되는 글꼴 조합은 [웹 안전 글꼴 조합을 참조하십시오.](https://www.w3schools.com/cssref/css_websafe_fonts.asp)



## font-style

`font-style` 속성은 주로 기울임 꼴 텍스트를 지정하는데 주로 사용됩니다.

이 속성에는 세가지 값이 있습니다.

- normal: 텍스트가 정상적으로 표시됩니다.
- italic: 텍스트는 기울임 꼴로 표시됩니다.
- oblique: 텍스트가 기울어집니다 (비스듬한 기울임 꼴과 유사하지만 덜 지원됩니다)

```css
p.normal {
    font-style: normal;
}

p.italic {
    font-style: italic;
}

p.oblique {
    font-style: oblique;
}
```

미리보기

<div style="font-style: normal">normal</div>
<div style="font-style: italic">italic</div>
<div style="font-style: oblique">oblique</div>


## font-size

`font-size` 속성은 텍스트의 크기를 설정합니다.

```css
body {
    font-size: 100%;
}
```


## font-weight

`font-weight` 속성은 글꼴의 두께를 지정합니다.

```css
p.normal {
    font-weight: normal;
}

p.thick {
    font-weight: bold;
}
```

## font-variant

`font-variant` 속성은 텍스트를 작은 대문자 글꼴로 표시할지 여부를 지정합니다.

작은 대문자 글꼴에서는 모두 소문자가 대문자로 변환됩니다. 그러나 변환 된 대문자는 텍스트의 원래 대문자보다 작은 글꼴 크기로 나타납니다.

```css
.small {
    font-variant: small-caps;
}
```

원본

```html
<div style="font-variant: small-caps">My name is Hege Refsnes.</div>
```

미리보기

<div style="font-variant: small-caps">My name is Hege Refsnes.</div>

## 단축속성

`font` 를 단축속성으로 한번에 지정할 수 있습니다.

```css
p.ex2 {
    font: italic bold 12px/30px Georgia, serif;
}
```

원본

```html
<div style="font: italic bold 12px/30px Georgia, serif;">This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph.</div>
```

미리보기

<div style="font: italic bold 12px/30px Georgia, serif;">This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph. This is a paragraph.</div>


