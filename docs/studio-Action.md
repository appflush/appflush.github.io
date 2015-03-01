---
title: App Studio - Action Window
layout: docs
section: docs/studio-Action
---

App Studio - Action Window
===================

이 문서에서는 각 아이템의 속성과 이벤트를 사용하는 방법을 설명 합니다.

<hr/>
<div class="space33"></div>

<div class="title row">
	액션 창
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong><span class="badge" style="background-color:#0000FF;">1</span> 점퍼</strong><br/>
		해당 아이템의 주소를 가지고 있어 드래그를 통해 다른 아이템와 연결 할 수 있다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#FF0000;">2</span> 아이템 주소</strong><br/>
		현재 아이템의 위치를 나타낸다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#380038;">3</span> 필터</strong><br/>
		속성과 이벤트의 이름을 검색해 매치되는 속성만 출력한다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#00FE00;">4</span> 필터 초기화</strong><br/>
		기존에 입력된 필터를 초기화 한다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#FEFE02;">5</span> 사용자 속성 추가</strong><br/>
		아이템에 새로운 사용자 속성을 추가 한다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#00FEFE;">6</span> 속성 추가</strong><br/>
		아이템이 가지고 있는 속성 리스트를 표시 한다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#808080;">7</span> 도움말</strong><br/>
		해당 속성의 도움말을 표시 한다
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#410241;">8</span> 도움말</strong><br/>
		입력된 속성을 저장하고 디바이스가 연결되어 있으면 디바이스에 전송한다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#0080C0;">9</span> 속성 드래그</strong><br/>
		입력된 속성을 다른 속성에 연결 할 수 있다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#FF007F;">10</span> 속성 드랍</strong><br/>
		현재 속성에 다른 아이템의 속성을 드랍 할 수 있다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#F7F7F7;color:black;">11</span> 스크립트</strong><br/>
		자주 사용되는 스크립트 아이템를 배치해 편리하게 아이템를 이벤트에 추가 할 수 있다.
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#030303;">12</span> 연결 아이템</strong><br/>
		다른 영역에서 생성된 아이템임을 알리는 표시
		<div class="space11"></div>
		<strong><span class="badge" style="background-color:#810202;">13</span> 제거</strong><br/>
		추가된 아이템를 제거한다.
		<div class="space11"></div>
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/property_main.png" data-lightbox="property_main" data-title="">
			<img src="/docs/images/property_main.png" alt=""/>
		</a>
		<a class="thumbnail" href="/docs/images/property_list.png" data-lightbox="property_list" data-title="추가 가능한 속성">
			<img src="/docs/images/property_list.png" alt=""/>
		</a>
		<a class="thumbnail" href="/docs/images/property_new.png" data-lightbox="property_new" data-title="사용자 속성 추가">
			<img src="/docs/images/property_new.png" alt=""/>
		</a>
	</div>
</div>
<div class="space33"></div>
<hr/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>속성 계층 슬라이드</strong><br/>
		각 아이템의 속성 및 이벤트는 다른 여러 아이템를 포함 할 수 있으며 각 속성창은 슬라이드 형태로 화면에 표시 된다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/property_slide.png" data-lightbox="property_slide" data-title="">
			<img src="/docs/images/property_slide.png" alt=""/>
		</a>
	</div>
</div>
<div class="space33"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	속성 및 이벤트
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-12">
		모든 UI 아이템는 속성과 이벤트를 통해 각 아이템의 모양을 변화시키고 사용자의 입력에 반응 한다.
	</div>
	<div class="movie col-xs-12 col-md-12">
		<iframe class="thumbnail" id="ytplayer" type="text/html" width="100%" height="720"
src="https://www.youtube.com/embed/7Jm9w6dVrqE?controls=1&enablejsapi=1&modestbranding=1&rel=0&showinfo=0&autohide=1&color=white&iv_load_policy=3&theme=light&vq=hd720"
frameborder="0" allowfullscreen></iframe>
	</div>
</div>
<div class="space33"></div>
<hr/>
<div class="space33"></div>
<div class="title row">
	글로벌<small>(전역)</small> 속성 아이템 연결
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-12">
		글로벌<small>(전역)</small> 속성 아이템를 연결해 사용 가능하다.<br/>
	</div>
	<div class="movie col-xs-12 col-md-12">
		<iframe class="thumbnail" id="ytplayer" type="text/html" width="100%" height="720"
src="https://www.youtube.com/embed/_Tk6-6cFY0w?controls=1&enablejsapi=1&modestbranding=1&rel=0&showinfo=0&autohide=1&color=white&iv_load_policy=3&theme=light&vq=hd720"
frameborder="0" allowfullscreen></iframe>
	</div>
</div>
<div class="space33"></div>
<hr/>
<div class="space33"></div>
<div class="title row">
	지역 속성 아이템 생성
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-12">
		윈도우 내에서만 존재하는 지역 속성 아이템를 생성 한다.<br/>
		이렇게 생성된 아이템는 윈도우를 close() 속성을 통해 닫으면 메모리에서 함께 제거 된다.
	</div>
	<div class="movie col-xs-12 col-md-12">
		<iframe class="thumbnail" id="ytplayer" type="text/html" width="100%" height="720"
src="https://www.youtube.com/embed/5Ek_i-6qCSA?controls=1&enablejsapi=1&modestbranding=1&rel=0&showinfo=0&autohide=1&color=white&iv_load_policy=3&theme=light&vq=hd720"
frameborder="0" allowfullscreen></iframe>
	</div>
</div>