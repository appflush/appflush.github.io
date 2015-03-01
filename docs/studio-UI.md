---
title: UI Items - UI Items
layout: docs
section: docs/studio-UI
---

App Studio - UI Items
===================

이 문서에서는 UI 아이템를 생성하고 배치하는 방법을 설명 합니다.

<hr/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<ul class="list-unstyled">
			<li>
				<strong>Root Container</strong><br/>
				컨테이너는 아이템를 자식으로 가질 수 있는 최상위 아이템이다. 모든 App은 하나 이상의 루트 컨테이너를 가진다. Window를 자식 아이템으로 가질 수 있다.
			</li>
			<li>
				<strong>Container</strong><br/>
				UI Controls를 자식으로 가질 수 있으며 화면의 레이아웃을 배치하고 시작적으로 표현 한다.
			</li>
			<li>
				<strong>UI Controls</strong><br/>
				각 아이템는 아이템 고유의 설정과 특수한 이벤트를 가지고 있다. 시각적인 요소를 통해 사용자와 직접적으로 상호작용이 가능하다.
			</li>
		</ul>
		<img class="iconEventItem" src="http://appflush.com/core/images/event_icon.png"> 표시는 사용자의 상호작용을 위한 이벤트에서 주소 사용되는 아이템이다.
		<div class="space11"></div>
		모든 아이템들은 마우스의 드래그를 이용해 아이템을 가질 수 있는 영역에 드랍해 생성한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/ui_3.jpg" data-lightbox="ui_3" data-title="">
			<img src="/docs/images/ui_3.jpg" alt=""/>
		</a>
	</div>
</div>

<div class="space33"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	아이템 생성
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-12">
		<ul>
			<li>
				<strong>글로벌 역역 (app 네임스페이스)</strong> <br/>
				글로벌 영역에 생성해 App내에 어디에서든 연결해 사용할 수 있는 아이템 이다.
			</li>
			<li>
				<strong>작업화면 (ui 네임스페이스)</strong><br/>
				윈도우, 뷰 등 자식을 가질 수 있는 아이템 내에서 생성해 해당 아이템 범위 안에서 사용할 수 있는 아이템 이다.
			</li>
			<li>
				<strong>속성 (ui 네임스페이스)</strong><br/>
				자식을 가질 수 있는 속성과 이벤트에 생성되는 아이템이다.
			</li>
		</ul>
	</div>
	<div class="movie col-xs-12 col-md-12">
		<iframe class="thumbnail" id="ytplayer" type="text/html" width="100%" height="720"
		src="https://www.youtube.com/embed/xycg2aoTEYY?controls=1&enablejsapi=1&modestbranding=1&rel=0&showinfo=0&autohide=1&color=white&iv_load_policy=3&theme=light&vq=hd720"
		frameborder="0" allowfullscreen></iframe>
	</div>
</div>
<div class="space33"></div>
<hr/>
<div class="space33"></div>
<div class="title row">
	네임스페이스
</div>

AppFlush에서 App메모리를 효율적으로 관리하기 위해 사용한다.

<div class="explain row">
	<div class="detail col-xs-12 col-md-12">
		<ul>
			<li>
				<strong>app 네임스페이스</strong> <br/>
				root Context에 선언되며 app이 종료 될 때 까지 메모리상에 상주한다.
			</li>
			<li>
				<strong>ui 네임스페이스</strong><br/>
				부모 Context에 선언되며 부모가 종료 될 때 함께 메모리에서 제거 된다. 글로벌 영역 이외의 모든 영역에서 아이템을 생성한 경우 사용된다.
			</li>
		</ul>
	</div>
	<div class="movie col-xs-12 col-md-12">
		<a class="thumbnail" href="/docs/images/studio_UI_code.png" data-lightbox="studio_UI_code" data-title="">
			<img src="/docs/images/studio_UI_code.png" alt=""/>
		</a>
	</div>
</div>