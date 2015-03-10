---
title: Template
layout: docs
section: docs/extend-template
---

Template <small>experimental</small>
===================

이 문서에서는 기존에 제작된 Titanium 코드를 AppFlush와 연결해 사용 할 수 있는 템플릿 기능을 설명 합니다.

<hr/>
<div class="space33"></div>

<div class="title row">
	템플릿
</div>

템플릿은 기존에 제작된 Titanium 코드를 AppFlush 플랫폼과 연동해 사용 할 수 있도록 하는 확장 기능 입니다. 템플릿을 사용하면 기존에 수많은 Titanium 오픈 코드를 손쉽게 AppFlush와 연결해 활용 하실 수 있습니다.

<div class="space33"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	동작 방식
</div>

기존에 제작된 소스 코드를 압축하여 템플릿 페이지에서 업로드 합니다. 서버에서는 업로드된 코드를 분석해 AppFlush와 연동하기 위한 코드로 사용하기 위해 commonJS 모듈 형식으로 변환 합니다.

1. 템플릿은 반드시 commonJS 모듈화 되어야 합니다.
1. 템플릿은 반드시 flush.js 파일을 포함해야 합니다.

<div class="space11"></div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">

	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/template_1.png" data-lightbox="template_1" data-title="">
			<img src="/docs/images/template_1.png" alt=""/>
		</a>
	</div>
</div>

<div class="space11"></div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">

	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/template_2.png" data-lightbox="template_2" data-title="">
			<img src="/docs/images/template_2.png" alt=""/>
		</a>
	</div>
</div>