---
title: App Studio - Script
layout: docs
section: docs/studio-script
---

App Studio - Script
===================

이 문서에서는 UI 아이템중 하나인 Script 아이템을 설명 합니다.

<hr/>
<div class="space33"></div>

<div class="title row">
	스크립트, 모듈
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<ul class="list-unstyled">
			<li>
				<img src="http://appflush.com/core/images/icon/icon_Modules.png"> <strong>CommonJS</strong><br/>
				독립 스코프를 사용하는 코드를 생성해 모듈화 한다. require 함수를 통해 호출 할 수 있다. JavaScript, Titanium API Code를 사용할 수 있다.
			</li>
			<li>
				<img src="http://appflush.com/core/images/icon/icon_NS_Script.png"> <strong>Script</strong><br/>
				JavaScript, Titanium API Code를 사용할 수 있다.
			</li>
		</ul>
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/script_main.png" data-lightbox="script_main" data-title="">
			<img src="/docs/images/script_main.png" alt=""/>
		</a>
	</div>
</div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		코드 에디터를 이용해 편리하게 코드를 작성할 수 있다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/script_function.png" data-lightbox="script_function" data-title="">
			<img src="/docs/images/script_function.png" alt=""/>
		</a>
	</div>
</div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>Script</strong> 에는 <strong>__clear</strong>라는 함수를 사용할 수 있다.
		<div class="space11"></div>
		<strong>__clear</strong>를 이용하면 새로고침시 디바이스에 중복으로 화면이 오픈되는 것을 방지할 수 있다. open() 메서드를 가진 rootContainer를 파라미터로 넘겨 사용 가능하다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/script_helper.png" data-lightbox="script_helper" data-title="">
			<img src="/docs/images/script_helper.png" alt=""/>
		</a>
	</div>
</div>

<div class="space33"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	드래그&드랍
</div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		드래그&드랍을 이용해 스크립트와 액션 윈도우를 함께 사용할 수 있다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/script_drop.png" data-lightbox="script_drop" data-title="">
			<img src="/docs/images/script_drop.png" alt=""/>
		</a>
	</div>
</div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		아이템을 스크립트에 드랍하면 커서가 있는 곳에 입력할 코드를 선택할 수 있는 옵션을 볼 수 있다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/script_dropDialog.png" data-lightbox="script_dropDialog" data-title="">
			<img src="/docs/images/script_dropDialog.png" alt=""/>
		</a>
	</div>
</div>

<div class="space33"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	스크립트 아이템
</div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		드랍된 아이템을 코드가 아닌 <a href="/docs/studio-Action.html">액션창</a>을 통해 아이템의 속성 및 이벤트를 변경할 수 있다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/script_script_item2.png" data-lightbox="script_script_item2" data-title="">
			<img src="/docs/images/script_script_item2.png" alt=""/>
		</a>
	</div>
</div>
