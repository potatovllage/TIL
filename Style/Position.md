<h1>CSS Postion</h1>

<h2>Position이란?</h2>

CSS Position 속성은 문서 상에 요소를 배치하는 방법을 지정한다. 
top,left,right,bottom 속성이 요소를 배치할 최종 위치를 결정한다.

<h2>Position 사용법</h2>

<h4>static</h4>

* 요소를 문서에 흐름에 맞춰 배치
* static은 position 속성의 기본값이다. 요소를 나열한 순서대로 배치하며 top, right, bottom, left와 같은 속성을 사용할 수 없다. (float 속성은 가능)

<h4>relative</h4>

* 이전 요소(주로 부모 요소)에 자연스럽게 연결하여 위치를 지정
* static이었을 때 배치되는 위치를 기준으로 상대적 위치를 지정할 수 있는 속성값이다. 

<h4>absolute</h4>

* 원하는 위치를 지정해 배치
* absolute 속성값은 브라우저가 문서의 흐름과 상관없이 (요소를 수직으로 쭉 놓을지, 수평으로 쭉 놓을지 등을 결정하는 것) left, right, top, bottom 속성값을 이용하여 요소를 위치시키는 속성값입니다. 
* 이때 기준이 되는 위치는 가장 가까운 부모 요소 혹은 조상 요소 중 position 속성이 relative인 요소입니다.

<h4>fixed</h4>

* 지정한 위치에 고정하여 배치
* fixed 속성값은 absolute 속성값과 마찬가지로 문서의 흐름과 상관없이 위치를 좌표로 결정한다.
* 하지만 position:relative인 제일 가까운 부모 혹은 조상 요소가 아닌 브라우저 창이 기준이 된다.
* 따라서 브라우저 창을 어디로 스크롤 하더라도 계속 고정되어 표시되게 된다. (기준점: 브라우저 왼쪽 위 꼭지점)

<h4>sticky</h4>

* 위치에 따라서 동작방식이 달라진다 요소가 임계점(scroll 박스 기준) 이전에   는 relative와 같이 동작 그 이후에는 fixed와 같이 동작한다
* 기준점을 설명하자면 top:50px인 sticky 속성을 예로 들어 스크롤을 내렸을 때 뷰포트(viewport)와 요소 사이의 거리가 50px 이상이면 relative처럼 동작하다 50px 이하가 됬을 때 기준점을 넘은 것으로 보고 그때부터 fixed 요소처럼 동작하게 된다 뷰포트(viewport)는 현재 사용자에게 보이는 브라우저 창이라고 생각하시면 된다
