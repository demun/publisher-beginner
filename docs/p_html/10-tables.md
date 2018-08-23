# Tables

표는 `<table>` 태그로 정의합니다.

각 테이블 행은 `<tr>` 태그로 정의됩니다.  
표 머리글은 `<th>` 태그로 정의됩니다.  
기본적으로 테이블 표제는 굵게 표시되고 중앙에 배치됩니다. 테이블 데이터/셀은 `<td>` 태그로 정의됩니다.

코드예:
```html
<table>
  <tr>
    <th>제목셀1</th>
    <th>제목셀2</th> 
    <th>제목셀3</th>
  </tr>
  <tr>
    <td>셀1</td>
    <td>셀2</td> 
    <td>셀3</td>
  </tr>
  <tr>
    <td>셀1</td>
    <td>셀2</td> 
    <td>셀3</td>
  </tr>
</table>
```

보여지는 예:

<table>
  <tr>
    <th>제목셀1</th>
    <th>제목셀2</th> 
    <th>제목셀3</th>
  </tr>
  <tr>
    <td>셀1</td>
    <td>셀2</td> 
    <td>셀3</td>
  </tr>
  <tr>
    <td>셀1</td>
    <td>셀2</td> 
    <td>셀3</td>
  </tr>
</table>


# caption
표에 제목을 사용할때 `caption` 을 사용합니다.  `<table>` 태그 바로 뒤에 위치합니다.

```html
<table>
  <caption>표의 제목</caption>
  ...
</table>
```

# summary
표 내용을 요약을 정의할때는 `summary` 속성을 사용합니다.

```html
<table summary="표 내용의 요약입니다">
...
</table>
```

# thead, tbody, tfoot

`<thead>` 태그는 HTML 표의 머리글 내용을 그룹화하는 데 사용됩니다. `<thead>` 요소에는 하나 이상의 `<tr>` 태그가 있어야합니다.  
`<tbody>` 태그는 본문 내용을 HTML 테이블에 그룹화하는 데 사용됩니다. `<tbody>` 요소에는 하나 이상의 `<tr>` 태그가 있어야합니다.  
`<tfoot>` 태그는 HTML 테이블의 꼬리말 내용을 그룹화하는 데 사용됩니다. `<tfoot>` 요소에는 하나 이상의 `<tr>` 태그가 있어야합니다. 
`<thead>`, `<tbody>` 및 `<tfoot>` 요소는 기본적으로 테이블 레이아웃에 영향을주지 않습니다.

코드예:
```html
<table>
	<thead>
		<tr>
			<th>제목1</th>
			<th>제목2</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>내용1</td>
			<td>내용2</td>
		</tr>
	</tbody>
	<tfoot>
		<tr>
			<td>꼬리글1</td>
			<td>꼬리글2</td>
		</tr>
	</tfoot>
</table>
```

보여지는예:
<table>
	<thead>
		<tr>
			<th>제목1</th>
			<th>제목2</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>내용1</td>
			<td>내용2</td>
		</tr>
	</tbody>
	<tfoot>
		<tr>
			<td>꼬리글1</td>
			<td>꼬리글2</td>
		</tr>
	</tfoot>
</table>




# colgroup, col
`<colgroup>` 태그는 서식 지정을 위해 표에 하나 이상의 열 그룹을 지정합니다.  
`<colgroup>` 태그는 `<table>` 요소의 하위 항목이어야 합니다.

`<col>` 태그는 `<colgroup>` 요소 내의 각 열에 대한 열 속성을 지정합니다 .  
`<col>` 태그는 각 행에 대해 각 셀의 스타일을 반복하는 대신 전체 열에 스타일을 적용하는 데 유용합니다.

`span` 속성은 `<col>` 요소가 확장되어야하는 열의 수를 지정합니다.

```html
<table>
  <colgroup>
    <col span="2" style="background-color:red">
    <col style="background-color:yellow">
  </colgroup>
  <tr>
    <th>제목1</th>
    <th>제목2</th>
    <th>제목3</th>
  </tr>
  <tr>
    <td>내용1</td>
    <td>내용2</td>
    <td>내용3</td>
  </tr>
</table>
```

보여지는예:

<table>
  <colgroup>
    <col span="2" style="background-color:red">
    <col style="background-color:yellow">
  </colgroup>
  <tr>
    <th>제목1</th>
    <th>제목2</th>
    <th>제목3</th>
  </tr>
  <tr>
    <td>내용1</td>
    <td>내용2</td>
    <td>내용3</td>
  </tr>
</table>



# colspan
colspan 은 열을 합쳐서 보여줍니다.

코드예:
```html
<table>
  <tr>
    <th>제목셀1</th>
    <th>제목셀2</th>
    <th>제목셀3</th>
  </tr>
  <tr>
    <td>셀1</td>
    <td colspan="2">셀2</td> 
  </tr>
  <tr>
    <td>셀1</td>
    <td>셀2</td> 
    <td>셀3</td>
  </tr>
</table>
```

보여지는 예:

<table>
  <tr>
    <th>제목셀1</th>
    <th>제목셀2</th>
    <th>제목셀3</th>
  </tr>
  <tr>
    <td>셀1</td>
    <td colspan="2">셀2</td> 
  </tr>
  <tr>
    <td>셀1</td>
    <td>셀2</td> 
    <td>셀3</td>
  </tr>
</table>


# rowspan
rowspan 은 여러행을 합쳐서 보여줍니다.

코드예:
```html
<table>
  <tr>
    <th>제목셀1</th>
    <th>제목셀2</th>
  </tr>
  <tr>
    <td>셀1</td>
    <td rowspan="2">셀2</td>
  </tr>
  <tr>
    <td>셀1</td>
  </tr>
</table>
```

보여주는 예:

<table>
  <tr>
    <th>제목셀1</th>
    <th>제목셀2</th>
  </tr>
  <tr>
    <td>셀1</td>
    <td rowspan="2">셀2</td>
  </tr>
  <tr>
    <td>셀1</td>
  </tr>
</table>