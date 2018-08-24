# `<form>`
HTML `<form>` 요소는 사용자 입력을 수집하는데 사용되는 양식을 정의합니다.  

`method="post"`, `method="get"` 폼 데이터를 제출할때 기본방법은 `get` 입니다.  
GET을 사용하면 제출된 양식 데이터가 페이지 주소 필드에 표시됩니다.  
POST는 제출된 양식 데이터를 페이지 주소 필드에 표시하지 않습니다. 중요한 정보나 개인 정보가 포함되어 있으면 항상 POST를 사용합니다. 

양식 요소는 텍스트 필드, 체크 박스, 라디오 버튼, 제출 버튼 등과 같은 입력 요소의 다른 유형입니다.

# `<input>`
`<input>` 요소는 유형 속성에 따라 여러 가지 방법으로 표시 될 수 있습니다.


- `<input type="text">` 는 텍스트 입력을 위한 한 줄 입력 필드를 정의합니다.
- `<input type="radio">` 는 라디오 버튼을 정의 합니다. 여러요소중 하나만 선택되어야 할때 사용합니다.
- `<input type="checkbox">` 는 체크 박스를 정의합니다. 여러요소를 선택해야할때 사용합니다.
- `<input type="submit">` 는 데이터양식을 처리자에게 제출하기 위한 버튼을 정의합니다.

확인란을 사용하면 제한된 수의 선택 항목 중 0 개 이상을 선택할 수 있습니다.

## 속성값

- `readonly`: 읽기만 가능하고 입력이 되지 않습니다.
- `disabled`: 비활성화 된 입력란은 사용할 수 없고 클릭 할 수 없으며 양식을 제출할 때 그 값은 전송되지 않습니다.
- `size`: 입력 필드(문자) 크기를 지정합니다.
- `maxlength`: 입력필드의 최대 길이를 지정합니다.



# `<select>`

`<select>` 는 드롭다운 목록을 나타냅니다.  
`<option>` 요소를 선택할 수있는 옵션을 정의합니다.  
기본적으로 드롭 다운 목록의 첫 번째 항목이 선택됩니다.

코드예:
```html
<select name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

보여지는 예:

<select name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>

`selected` 속성은 선택한 속성으로 정의됩니다.
`size` 는 기본적으로 `size`에서 지정한 숫자만큼 보여집니다.
`multiple` 속성은 다중선택을 허용합니다.


# `<textarea>`
`<textarea>` 요소는 여러 줄의 입력 필드를 정의할 때 사용합니다.

코드예:
```html
<textarea name="message" rows="10" cols="30">
이곳은 텍스트에어리어 입니다.
</textarea>
```

보여지는 예:

<textarea name="message" rows="10" cols="30">
이곳은 텍스트에어리어 입니다.
</textarea>


# `<button>`
`<button>` 요소는 클릭 버튼을 정의합니다.



# `<fieldset>`
`<fieldset>` 요소 형태로 그룹과 관련된 데이터를 사용한다.  
`<legend>` 엘리먼트는 `<fieldset>` 요소에 대한 자막을 정의한다.

코드예:
```html
<form>
  <fieldset>
    <legend>정보 입력:</legend>
    이름:<br>
    <input type="text" name="이름" value=""><br>
    ...
  </fieldset>
</form>
```

보여지는 예:

<form>
  <fieldset>
    <legend>정보 입력:</legend>
    이름:<br>
    <input type="text" name="이름" value=""><br>
    ...
  </fieldset>
</form>

