# display

`display` 속성은 요소가 표시되는지 여부를 지정합니다.

속성 | 설명 
---------- | -----------
inline | 기본값. 요소를 인라인 요소 (예: `<span>`)로 표시합니다. 높이 및 너비 속성은 아무 효과가 없습니다.
block | 요소를 `<p>`와 같은 블록 요소로 표시합니다. 새 줄에서 시작하여 전체 너비를 차지합니다.
inline-block | 요소를 인라인 수준 블록 컨테이너로 표시합니다. 요소 자체는 인라인 요소로 형식화되지만 높이 및 너비 값을 적용 할 수 있습니다.
inline-table | 요소가 인라인 수준 테이블로 표시됩니다.
list-item | 요소가 `<li>` 요소처럼 동작하도록 합니다.
run-in | 요소를 문맥에 따라 블록 또는 인라인으로 표시합니다.
table | 요소가 `<table>` 요소처럼 동작하도록 합니다.
table-caption | 요소가 `<caption>` 요소처럼 동작하도록 합니다.
table-column-group | 엘리먼트가 `<colgroup>` 엘리먼트처럼 동작하도록 합니다.
table-header-group | 요소가 `<thead>` 요소처럼 동작하도록 합니다.
table-footer-group | 요소가 `<tfoot>` 요소처럼 동작하도록 합니다.
table-row-group | 요소가 `<tbody>` 요소처럼 동작하도록 합니다.
table-cell | 요소가 `<td>` 요소처럼 동작하도록 합니다.
table-column | 엘리먼트가 `<col>` 엘리먼트처럼 동작하도록 합니다.
table-row | 요소가 `<tr>` 요소처럼 동작하도록 합니다.
none | 요소가 완전히 제거되었습니다.
initial | 이 속성을 기본값으로 설정합니다.
inherit | 부모 요소에서이 속성을 상속받습니다.

```css
span {
  display: block;
}
```


# visibility

`visibility` 속성은 요소가 표시되는지 여부를 지정합니다.

속성 | 설명 
---------- | -----------
visible | 기본값. 요소가 표시됩니다.
hidden | 요소가 보이지 않습니다 (그러나 여전히 공간을 차지함).
collapse | 표 요소에 대해서만 접기는 행이나 열을 제거하지만 표 레이아웃에는 영향을주지 않습니다. 행 또는 열에 의해 차지한 공간은 다른 내용에 사용할 수 있습니다. 축소가 다른 요소에서 사용되면 'hidden'으로 렌더링됩니다.
initial | 이 속성을 기본값으로 설정합니다.
inherit | 부모 요소에서이 속성을 상속받습니다.


```css
.class {
  visibility: hidden;
}
```
