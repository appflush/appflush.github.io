---
title: Device Message Push
layout: docs
section: docs/distribute-push
---

Device Message Push <small>experimental</small>
===================

이 문서에서는 배포된 App에 푸시 메세지를 보내는 방법을 설명 합니다.

<hr/>
<div class="space33"></div>

<div class="title row">
	푸시 메세지
</div>

App을 설치한 디바이스에 원격으로 메세지를 전달 하는 원격 알림 서비스 입니다.

<div class="space33"></div>

<div class="space11"></div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		프로젝트 관리 화면 Action 버튼의 Push 버튼 클릭
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/push_1.png" data-lightbox="push_1" data-title="">
			<img src="/docs/images/push_1.png" alt=""/>
		</a>
	</div>
</div>

<div class="space33"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	Android
</div>

<div class="space11"></div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>Content Title</strong><br>
		<ul>
			<li>App의 StatusBar에 표시</li>
			<li>App실행 후 Alert Dialog 창의 title</li>
		</ul>
		<strong>Content Text</strong><br>
		<ul>
			<li>App실행 후 Alert Dialog 창의 안내 메세지</li>
		</ul>
		<strong>Options</strong><br>
		<ul>
			<li>팝업 메세지 열기
				<ul>
					<li>App실행시 Alert Dialog 생성</li>
				</ul>
			</li>
			<li>특정 윈도우 열기
				<ul>
					<li>App실행시 선택된 윈도우 열기</li>
				</ul>
			</li>
		</ul>
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/push_2.png" data-lightbox="push_2" data-title="">
			<img src="/docs/images/push_2.png" alt=""/>
		</a>
		<a class="thumbnail" href="/docs/images/push_4.png" data-lightbox="push_4" data-title="">
			<img src="/docs/images/push_4.png" alt=""/>
		</a>
		<a class="thumbnail" href="/docs/images/push_5.png" data-lightbox="push_5" data-title="">
			<img src="/docs/images/push_5.png" alt=""/>
		</a>
	</div>
</div>

<div class="space33"></div>
<hr/>
<div class="space33"></div>
<div class="title row">
	iOS
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>Content Title</strong><br>
		<ul>
			<li>App실행 후 Alert Dialog 창의 title</li>
		</ul>
		<strong>Content Text</strong><br>
		<ul>
			<li>App실행 후 Alert Dialog 창의 안내 메세지</li>
		</ul>
		<strong>Options</strong><br>
		<ul>
			<li>팝업 메세지 열기
				<ul>
					<li>App실행시 Alert Dialog 생성</li>
				</ul>
			</li>
			<li>특정 윈도우 열기
				<ul>
					<li>App실행시 선택된 윈도우 열기</li>
				</ul>
			</li>
			<li>아이콘 배찌
				<ul>
					<li>App icon에 나타낼 배찌</li>
				</ul>
			</li>
		</ul>
		<strong>Appkey</strong><br>
		해당 App의 appkey
		<div class="space11"></div>
		<strong>Appkey password</strong><br>
		Appkey의 비밀번호
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/push_3.png" data-lightbox="push_3" data-title="">
			<img src="/docs/images/push_3.png" alt=""/>
		</a>
</div>