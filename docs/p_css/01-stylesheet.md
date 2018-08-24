# stylesheet

스타일시트는 `.css` 확장자로 `css` 구문으로 작성된 파일을 말합니다.

CSS 는 다음 세 가지 방법으로 HTML 요소에 추가 할 수 있습니다.

- 외부 스타일
- 내부 스타일
- 인라인 스타일

## 외부 스타일

`<head>` 태그안에 `<link>` 요소로 스타일을 참조하는 방식으로 가장 많이 사용하는 방법입니다.

```html
<head>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
```

## 내부 스타일

`<head>` 태그안에 `<style>`요소로 `css` 를 추가하는 방식입니다.

```html
<head>
  <style>
    body {
      background-color: white;
    }
  </style>
</head>
```

## 인라인 스타일

인라인 스타일은 `html` 태그에 `style` 속성을 사용하여 추가하는 방법입니다.

```html
<h1 style="background-color: white">내용</h1>
```

## 구문

css 구문은 선택자와 속성:값으로 구성됩니다.

![css rule](../../img/css-rule.gif)

선택자는 `html` 요소를 말하며, 반드시 중괄호{} 로 묶습니다.

# selector

선택자는 html 태그이름, ID, class, 속성 등에 사용할 수 있습니다.

## 태그 선택자

html 요소를 말합니다.

```css
p {
  color: red;
}
```

모든 `<p>` 태그에 컬러가 빨강색이 됩니다.

## ID 선택자

id 선택자는 html 요소에 id 속성을 부여해서 사용합니다.

id 는 해당페이지에서 고유한 요소에 사용합니다. 한번만 사용할 수 있습니다.

id 는 해시(#) 다음에 id 를 씁니다.

```css
#header {
  color: red;
}
```

> id 는 숫자로 시작할 수 없습니다.

## 클래스 선택자

클래스 선택자는 html 요소에 class 속성을 부여해서 사용합니다.

클래스는 다중으로 사용할수 있습니다.

클래스는 마침표(.) 다음에 클래스를 씁니다.

```css
.header {
  color: red;
}
```

> class 는 숫자로 시작할 수 없습니다.

## 주석

css 에서 주석은 `/*` 시작해서 `*/` 로 닫습니다.

```css
/* 이글은 css 내에서 보이지 않습니다. */

/* 
이글은 css 내에서 보이지 않습니다. 
*/
```

### 상속

CSS 에서 어려움을 겪는 것이 바로 `상속` 와 `우선순위` 입니다.  
CSS 에서 상속이란 부모요소에 지정한 스타일이 자식요소에 적용되는 것을 말합니다.

예를들어 아래와같은 html 구조가 있다고 합니다.

```html
<ul>
    <li>자식요소1</li>
    <li>자식요소2</li>
    <li>자식요소3</li>
</ul>
```

여기서 `<ul>` 요소는 `<li>` 요소의 부모입니다. 즉 `<li>` 요소는 `<ul>` 요소의 자식입니다.  
`<ul>:부모` `<li>:자식` 관계입니다.

부모인 ul 요소에 스타일을 주면 자식인 li 에 스타일이 상속이 됩니다.

일반적으로 body 에 글꼴 스타일을 적용하면 문서내의 모든 요소에 스타일이 적용이 됩니다.  
따로 하위요소에 스타일을 지정하지 않으면 body 요소에 적용된 스타일이 적용됩니다.

![css rule](../images/child.jpg)

### 우선순위

스타일시트는 다음과 같은 3 개의 CSS 원천 소스(original source)를 가질수 있습니다.

- 제작자(author) 원천 소스: 웹사이트 제작자가 지정하는 자신의 페이지 스타일
- 사용자(user) 원천 소스: 사용자가 직접 정하는 자신의 사용할 스타일
- 사용자 도구(user agent) 원천 소스: 웹 브라우저 자체에 지정된 기본 스타일

##### 원천 소스 우선 순위

!important 선언을 한 사용자 스타일 > !important 선언을 한 제작자 스타일 > 제작자 스타일 > 사용자 스타일 > 사용자 도구 선언 (브라우저 자체의 선언)

##### CSS 명시도(Specificity) 계산법

> !important > id[100] > class[10] > tag[1] > \*[0]

선택자에 따른 점수

<table class="table">
    <tr>
        <th>지정방법</th>
        <th>예제</th>
        <th>점수</th>
    </tr>
    <tr>
        <td>전체선택자</td>
        <td>\*</td>
        <td>0점</td>
    </tr>
    <tr>
        <td>태그선택자</td>
        <td>ul</td>
        <td>1점</td>
    </tr>
    <tr>
        <td>가상클래스속성</td>
        <td>:first-child</td>
        <td>10점</td>
    </tr>
    <tr>
        <td>속성선택자</td>
        <td>a[href*="sample"]</td>
        <td>10점</td>
    </tr>
    <tr>
        <td>클래스선택자</td>
        <td>.sample</td>
        <td>10점</td>
    </tr>
    <tr>
        <td>id선택자</td>
        <td>#sample</td>
        <td>100점</td>
    </tr>
    <tr>
        <td>인라인스타일</td>
        <td>style=""</td>
        <td>1000점</td>
    </tr>
    <tr>
        <td>!important</td>
        <td>!important</td>
        <td>10000점</td>
    </tr>
</table>

선택자의 원리에 따른 점수계산

- a = 선택자중 ID 의 수를 세어 100 자리에 놓는다,
- b = 선택자중 가상 클래스와 클래스의 수를 세어 10 자리에 놓는다.
- c = 선택자중 엘리먼트의 수를 세어 1 의 자리에 놓는다.
- d = 가상 엘리먼트는 무시한다.

<table class="table">
    <tr>
        <th></th>
        <th>a(100자리)</th>
        <th>b(10자리)</th>
        <th>c(1자리)</th>
        <th>계산방법</th>
        <th>점수</th>
    </tr>
    <tr>
        <td>*</td>
        <td>0</td>
        <td>0</td>
        <td>0</td>
        <td>전체선택자 1개</td>
        <td>0</td>
    </tr>
    <tr>
        <td>li</td>
        <td>0</td>
        <td>0</td>
        <td>1</td>
        <td>태그선택자 1개</td>
        <td>1</td>
    </tr>
    <tr>
        <td>ul li</td>
        <td>0</td>
        <td>0</td>
        <td>2</td>
        <td>태그선택자 2개</td>
        <td>2</td>
    </tr>
    <tr>
        <td>ul ol+li</td>
        <td>0</td>
        <td>0</td>
        <td>3</td>
        <td>태그선택자 3개</td>
        <td>3</td>
    </tr>
    <tr>
        <td>li.num</td>
        <td>0</td>
        <td>1</td>
        <td>1</td>
        <td>태그선택자 1개 클래스선택자 1개</td>
        <td>11</td>
    </tr>
    <tr>
        <td>ul+ol li.num</td>
        <td>0</td>
        <td>1</td>
        <td>3</td>
        <td>태그선택자 1개 클래스선택자 3개</td>
        <td>13</td>
    </tr>
    <tr>
        <td>li.num.last</td>
        <td>0</td>
        <td>2</td>
        <td>1</td>
        <td>태그선택자 1개 클래스선택자 2개</td>
        <td>21</td>
    </tr>
    <tr>
        <td>#sample</td>
        <td>1</td>
        <td>0</td>
        <td>0</td>
        <td>아이디선택자 1개</td>
        <td>100</td>
    </tr>
    <tr>
        <td>p#sample</td>
        <td>1</td>
        <td>0</td>
        <td>1</td>
        <td>태그선택자 1개 아이디선택자 1개</td>
        <td>101</td>
    </tr>
</table>

### CSS3 와 CSS 모듈

CSS 가 스타일 시트의 기본이 되면서 CSS1 을 거쳐 CSS2 가 개발되어 스타일 시트가 많이 알려졌고 지금까지 사용되고 있습니다.

HTML5 가 개발되면서 CSS3 기술도 함께 개발되고 있는데 좀더 화려한 화면을 구성할수 있고 에니메이션까지 지원합니다.

CSS3 부터는 배경이나 글꼴, 박스 모델 등 수십 개 기능을 주제별로 규약을 따로 만들었고 이것을 "CSS 모듈" 이라고 합니다.

이처럼 모듈별로 진행이 되기 때문에 표준이 된것도 있고, 계속 진행중인것도 있습니다.

[http://www.w3.org/Style/CSS/](http://www.w3.org/Style/CSS/) 에 접속하면 왼쪽에 LC, WD, CR, PR, REC 등 진행상태에 대한 표시를 볼 수 있습니다.

- LC(Last Call Working Draft, 최종검토): 초안을 최종 검토하는 단계입니다.
- WD(Working Draft, 초안): W3C 가 그 멤버뿐만 아니라 대중, 다른 기술단체 등 여러 커뮤니티의 검토를 받기위해 공개한 문서입니다.
- CR(Candidate Recommendation, 후보 권고안): 광범위하게 검토받고 워킹그룹의 기술적 요구사항을 만족시킨 것이 검증된 문서로 W3C 는 더 많은 구현 경험을 얻기 위해 이 문서를 대중에게 공개합니다.
- PR(Proposed Recommendation, 제안 권고안): 광범위한 기술적 구현과 검토가 끝나 거의 완성된 문서로 최종 승인을 얻기 위해 자문위원회에 보내집니다.
- REC(W3C Recommentation, 권고안): 모든 합의를 끝낸 후 W3C 멤버들과 감독의 승인을 받은 문서로 W3C 에서 이 문서가 널리 쓰이길 권장하는 표준 권고안입니다.

#### CSS3 와 접두사(prefix)

표준 규약이 되지 않은 속성들은 브라우저에 따라 다른 방식으로 지원되기 때문에 속성 이름 앞에 접두사(prefix)를 붙여 브라우저별로 구분해야 합니다.

주로 사용하는 브라우져 접두사는 다음과 같습니다.

<table class="table">
    <tr>
        <th>접두사</th>
        <th>설명</th>
    </tr>
    <tr>
        <td>-webkit</td>
        <td>웹킷 방식의 브라우저용(사파리, 크롬)</td>
    </tr>
    <tr>
        <td>-moz</td>
        <td>게코 방식 브라우저용(모질라 파이어폭스)</td>
    </tr>
    <tr>
        <td>-o</td>
        <td>오페라 브라우저</td>
    </tr>
    <tr>
        <td>-ms</td>
        <td>마이크로소프트 인터넷 익스플로러</td>
    </tr>
</table>

접두사를 쓸때는 브라우져 접두사를 먼저쓰고 표준이 정해진 후 사용할 표준속성을 나중에 지정합니다.

```css
.sample {
  -webkit-transform: rotate(15deg);
  -moz-transform: rotate(15deg);
  -o-transform: rotate(15deg);
  -ms-transform: rotate(15deg);
  transform: rotate(15deg);
}
```

### 문서 보는 법

이 방식은 CSS 규약본 원서에도 나오는 방식으로 몇가지 규칙이 있습니다.

##### 값

이 부분은 그 속성들에 유효한 값을 지정한다. 값 종류(type)들은 여러가지 방법으로 지정될 수 있다.

- 키워드(keyword) 값들(예: auto, disc, 등)
- 기본 테이터 타입들은 "<"와 ">"사이에 나타난다(예: <길이>, <백분율>, 등).
- 같은 이름을 갖고 속성값들 범위가 같은 종류(예: <'border-width'> <'background-attachment'>, 등). 이 경우, 그 종류(type) 이름은 그 속성 이름으로 "<" 와 ">"사이에서 따옴표 안에 표시하였다(예: <'border-width'>).
- 같은 이름을 속성으로 사용하지 않는 비 터미날들의 경우, 그 비 터미날 이름은 "<" 와 ">"사이에 <border-width>와 같이 표현 하였다.

이들 정의들에 있는 따옴표 없이(예: red) 그대로 나타나는 다른 단어들은 키워드(keyword) 들이다. 슬래쉬(/)와 컴마(,) 또한 그래도 나타나야 한다.

값은 다음과 같이 정렬될 수 있습니다.

- 여려개의 나란히 놓인 단어들은 모두 주어진 순서로 나타나야 한다.
- 바(|) 로 구분된 두개이상은 선택적으로 사용할 수 있는것으로 그들 중 한개가 정확히 나타나야 한다.
- 이중바(||) 로 구분된 두개이상 선택사항은 그중 한개이상이 어떤 순서로든 나와야 한다.
- 괄호([ ])는 그룹을 짓기 위한 것이다.

나란히 놓인 단어들은 이중바(||)보다 우선하고, 이중바(||)는 바(|)보다 우선한다.

우선순위를 보면 `연속된 단어 > || > |` 순이다.

다음 두 줄은 동등하다.

```css
ab | c || de
[ab] | [c || [de]]
```

각각의 유형(type), 키워드(keyword), 또는 괄호로 묶인 그룹 다음에는 다음의 수정자(modifier)들이 올 수 있다.

- 별표(\*)는 앞의 타입, 단어, 그룹이 한번도 안나오던가 여러번 나올 수 있다.
- 플러스(+)는 앞의 타입, 단어, 그룹이 한번이상 나옴을 나타낸다.
- 물음표(?)는 앞의 타입, 단어, 그룹이 선택적이다.
- 대괄호 안의 짝({A,B})은 앞의 타입, 단어, 그룹이 최소 A 번, 최대 B 번을 나타낸다.

##### initial

이 부분은 그 속성의 최초값을 지정한다. 만일 그 속성이 상속(inherit)된 것이면, 이는 문서의 최상위 엘리먼트에서 주어진 값이다.

##### inherit

이 부분을 그 속성값이 조상(ancestor) 엘리먼트로 부터 상속(inherit)된 것인가를 나타낸다.

일부 값들은 문서계통에서 그 엘레멘트의 자식(child)에 상속(inherit)된다. 각 속성은 이들이 상속되는가 않되는가를 정의한다.

<br>
