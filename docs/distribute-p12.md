---
title: 인증서 변환
layout: docs
section: docs/distribute-p12
---

PKCS 12 Format
===================

이 문서에서는 OSX 키체인 상에서 Apple 개발자 인증서를 생성한 경우, 해당 인증서를 PKCS 12 포맷으로 추출하는 방법을 설명 합니다.

<hr/>
<div class="space33"></div>

<div class="title row">
	비밀키 추출
</div>

OSX 상에서 생성된 비밀키를 PKCS 12 포맷으로 추출하는 방법을 설명 합니다. 이 파일은 AppFlush에서 발급한 Private Key를 대신해 사용 합니다.

<div class="space11"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		키체인에 기존에 생성한 개인 키를 추출한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/p12_export.png" data-lightbox="p12_export" data-title="">
			<img src="/docs/images/p12_export.png" alt=""/>
		</a>
	</div>
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		개인 정보 교환(.p12) 포맷으로 저장한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/p12_save.png" data-lightbox="p12_save" data-title="">
			<img src="/docs/images/p12_save.png" alt=""/>
		</a>
	</div>
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		6자리 이상의 비밀번호를 입력 합니다. <strong>AppKey</strong>생성시에 사용된다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/p12_pass.png" data-lightbox="p12_pass" data-title="">
			<img src="/docs/images/p12_pass.png" alt=""/>
		</a>
	</div>
</div>

<div class="title row">
	AppKey 발급
</div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		위에서 생성한 개인 정보 교환(.p12) 파일은 Private Key를 대신한다.
		<div class="space11"></div>
		<strong>추출시 입력한 비밀번호를 AppKey 비밀번호로 입력한다.</strong>
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/p12_use.png" data-lightbox="p12_use" data-title="">
			<img src="/docs/images/p12_use.png" alt=""/>
		</a>
	</div>
</div>