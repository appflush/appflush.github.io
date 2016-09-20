---
title: Create Project
layout: docs
section: docs/project-create
---

Create Project
===================

이 문서에서는 프로젝트를 생성하고 수정 하는 방법을 설명 합니다.

하나의 프로젝트는 하나의 App을 생성하는 것과 같으며, 프로젝트 생성시에는 App을 생성할때 필요한 정보들을 입력해 주어야 합니다.

<hr/>
<div class="space33"></div>

<div class="title row">
	프로젝트 생성
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-4">
		<dl>
			<dt>Project Name</dt>
			<dd>프로젝트를 구분하는 이름, 공백이 없는 영문자 숫자의 조합</dd>
			<dt>App Title</dt>
			<dd>App의 이름 입니다. App을 설치시에 아이콘과 함께 표시 되는 이름</dd>
			<dt>App id</dt>
			<dd>App의 패키지 이름이자 고유 이름 <small><a href="#appid">[자세히]</a></small></dd>
			<dt>App Version</dt>
			<dd>App의 버전 관리</dd>
			<dt>Publisher</dt>
			<dd>제작자 정보</dd>
			<dt>Copyright</dt>
			<dd>제작된 결과물의 저작권 정보</dd>
			<dt>Web Site</dt>
			<dd>제작자 웹사이트 주소</dd>
			<dt>App Description</dt>
			<dd>저작물의 자세한 정보</dd>
			<dt>Divice OS</dt>
			<dd>제작할 OS 종류 선택</dd>
			<dt>Private</dt>
			<dd>프로젝트의 공개, 비공개 설정 <small><a href="#private">[자세히]</a></small></dd>
		</dl>

	</div>
	<div class="movie col-xs-12 col-md-8">
		<iframe class="thumbnail" id="ytplayer" type="text/html" width="600" height="720"
src="https://www.youtube.com/embed/ths3i_-3MJU?controls=1&enablejsapi=1&modestbranding=1&rel=0&showinfo=0&autohide=1&color=white&iv_load_policy=3&theme=light&vq=hd720"
frameborder="0" allowfullscreen></iframe>
	</div>
</div>

<div class="space11"></div>
<hr/>
<div class="space11"></div>

<strong id="appid">App ID 명명 규칙</strong>

1. 모든 App은 App ID를 가지고 있으며 모든 App의 App ID는 중복될 수 없습니다.
1. App ID는 App을 마켓이나 스토어에 등록시 요구되는 값으로 반드시 <strong>마침표(.) 를 포함한 고유한 값</strong>이어야 합니다.
1. 공백 및 특수문자를 사용하실 수 없습니다.
1. 모두 소문자로 입력되어야 하며 대문자를 입력할 경우 Android 환경에서 정상적으로 동작하지 않습니다.
1. 반드시 마침표(.) 를 이용해야 하며 "testapp" 과 같이 마침표를 사용하지 않을 경우 사용할 수 없습니다.
1. 우리는 Java 패키지 이름과 같은 방식을 추천 합니다. 예를 들면 com.yourdomain.yourappname 와 같이 도메인을 거꾸로 사용하여 고유한 값을 만들 수 있습니다. 도메인이 없다면 여러분의 이름이나 별명을 사용해도 됩니다. 하지만 다른 사람들과 중복될 염려가 있을 경우 사용해서는 안됩니다.

<strong>유의사항</strong>

- 생성된 프로젝트의 App ID는 변경 할 수 없습니다.
- Android 사용시 주의사항
	1. "package", "case" 같은 Java 키워드를 사용할 수 없습니다.
- iOS 사용시 주의사항
	1. App ID는 iOS Provisioning Portal, iTunes Connect와 일치하게 생성 되어야 합니다.

<div class="space11"></div>
<hr/>
<div class="space11"></div>

<strong id="private">비공개 프로젝트 만들기</strong>

1. 비공개 프로젝트를 만들고자 할 경우 Basic License 이상으로 <a href="//auth.appflush.com/myAccount/billLicense?active=22">업그레이드</a> 해야 합니다.

<div class="space11"></div>
<hr/>
<div class="space11"></div>