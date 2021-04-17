## display

div 태그는 block 으로 화면에 표시되고, span은 인라인으로 화면에 표시된다.

기본 속성은 위와 같은데, display로 기본으로 지정된 위 형태들을 바꿔줄 수 있다.

```css
div , span{
    width: 80px;
    height: 80px;
    margin: 20px;
}

div{
    background-color: pink;
    display: inline;
}
span{
    background-color: green;
    display: block;
}
```
inline이나, block 외에도 inline-block이라는 것이 존재하는데, 이것은 박스를 만들어주는데 그 박스를 인라인으로 배치하는 특별한 박스이다.인라인의 경우, 컨텐츠의 사이즈만을 차지했었는데, display 에 inline-block 속성을 적용함으로써 지정한 너비와 높이에 맞게 박스영역을 차지하며 출력된다.

REMEMBER : 
`inline`: 물건
`inline-block`: 박스인데 한 줄에 여러개가 진열될 수 있는 특별한 박스
`block` : 상자인데, 한 줄당 하나만 들어가는 상자

## position
position 만 잘 이해해도 나중에 웹사이트 만들때 박스를 쉽게 배치할 수 있음

position은 기본 값으로 static을 가지고 있음. 즉 굳이 명시하지 않아도 `position: static`임

### positon value
`static` : 굳이 적어주지 않아도 position: static. 디폴트 값. 요소를 나열한 순서대로 배치하며 top, right, bottom, left와 같은 속성을 사용할 수 없다
`relative` : static이었을 때 배치되는 위치를 기준으로 상대적 위치를 지정할 수 있다.
`absolute` : 가장 가까운 부모요소 혹은 조상요소 중 position 속성이 relative인 요소를 기준으로 배치
`fixed` : 브라우저 창을 기준으로 배치
`sticky` : 스크롤을 해도, 자리에 딱 붙어있음.

