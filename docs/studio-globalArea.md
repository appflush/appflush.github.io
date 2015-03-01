---
title: App Studio - Global Area
layout: docs
section: docs/studio-globalArea
---

App Studio - Global Area
===================

이 문서에서는 App Studo의 글로벌 영역 인터페이스를 설명 합니다.

글로벌 영역은 root Context에 선언되는 아이템 입니다. 이곳에 드래그 되어 생성되는 아이템은 App의 어떤 아이템에서도 접근 가능합니다. 여러 윈도우, 탭그룹 등에서 동시에 사용하고자 할 경우 사용됩니다. 하지만 app이 종료되기 전까지 디바이스의 메모리에 상주 합니다.

<hr/>
<div class="space33"></div>

<div class="title row">
	글로벌 아이템 영역
</div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		Drag&Drop을 통해 모든 생성 가능한 아이템들을 Root Context에 생성한다. 여기에 생성되는 아이템은 모든 하위 아이템에서 참조하여 사용할 수 있다. 글로벌 영역의 아이템은 앱이 종료되기 전까지 메모리에 상주한다.
		<div class="space11"></div>
		글로벌 아이템은 실행시에 왼쪽 아이템부터 오른쪽 아이템으로 순차적으로 실행 되며 드래그&드랍으로 실행 순서를 변경 할 수 있다.
		<div class="space11"></div>
		<img src="http://appflush.com/core/images/firstOpenWindow.png" alt=""/> 배포용으로 빌드된 App이 가장 먼저 실행할 아이템을 지정한다. 지정하지 않으면 아무것도 실행하지 않는다. 단, 글로벌 영역에 Script와 Module은 실행된다.

	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_global_area.png" data-lightbox="studio_global_area" data-title="">
			<img src="/docs/images/studio_global_area.png" alt=""/>
		</a>
	</div>
</div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>글로벌 아이템 옵션</strong>
		<div class="space11"></div>
		<dl>
			<dt>Open</dt>
			<dd>App Studio상에서 편집할 수 있게 불러 온다.</dd>
			<dt>Send</dt>
			<dd>연결된 디바이스에 아이템을 전송해 디바이스에 적용 한다.</dd>
			<dt>Property</dt>
			<dd>속성 및 이벤트를 수정하기 위한 액션창을 화면에 표시한다.</dd>
			<dt>First</dt>
			<dd>해당 아이템을 App 빌드시에 제일 처음 실행되도록 한다.</dd>
			<dt>TreeView</dt>
			<dd>아이템의 자식 아이템을 Tree형태로 표시한다.</dd>
			<dt>Rename</dt>
			<dd>아이템의 이름을 변경한다.</dd>
			<dt>Remove</dt>
			<dd>아이템을 삭제 한다.</dd>
		</dl>
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_window_options.png" data-lightbox="studio_window_options" data-title="">
			<img src="/docs/images/studio_window_options.png" alt=""/>
		</a>
	</div>
</div>

<div class="space44"></div>