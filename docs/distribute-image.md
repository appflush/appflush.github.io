---
title: Icon & Splash image
layout: docs
section: docs/distribute-image
---

Icon & Splash image
===================

이 문서에서는 App을 배포하기 위한 스플래시 이미지 및 아이콘 규격을 설명 합니다.

<hr/>
<div class="space33"></div>


**아이콘**

App의 정체성을 나타내는 대표 이미지입니다. App을 실행 하기 위해 누르는 버튼이미지 입니다.

<img class="thumbnail" src="/docs/images/splash_1.png" alt=""/>

<div class="space11"></div>

**스플래시 이미지**

App은 실행시에 데이타를 메모리에 로드하는 과정이 필요 합니다. 이 과정에서 로딩 이미지를 미리 출력하는데 이때 출력되는 이미지를 스플래시 이미지라고 합니다. 잘 디자인된 스플래시 이미지는 App의 퀄리티를 한층 높여 주고 App의 첫 인상에도 좋은 영향을 줍니다.

<img class="thumbnail" src="/docs/images/splash_0.png" alt=""/>

<div class="space11"></div>

**자동화**

Android와 iOS의 경우 서로 다른 디바이스와 스크린 사이즈를 고려해 여러 해상도의 아이콘과 스플래시 이미지를 만들어야 합니다. 이러한 작업은 적지 않은 노력이 요구 됩니다. 하지만 AppFlush에서는 다음 규격을 맞춰 업로드 하면 이러한 작업을 <a href="https://github.com/FokkeZB/TiCons" target="_blank" class="btn btn-link">TiCons <i class="fa fa-external-link"></i></a>를 통해 자동으로 처리 합니다.

<div class="space11"></div>

**규격**

1. 아이콘, 스플래시 이미지 모두 PNG 포맷
1. 아이콘
	* 512x512 or 1024x1024
	* <a href="http://site.appflush.com/assets/boot/appflush_appicon.png" target="_blank" class="btn btn-link">예제(example) <i class="fa fa-external-link"></i></a>
1. 스플래시 이미지
	* 정 중앙 1000x1000 pixels 안에 디자인 배치된 2208x2208 크기의 이미지
	* <a href="http://site.appflush.com/assets/boot/appflush_splash.png" target="_blank" class="btn btn-link">예제(example) <i class="fa fa-external-link"></i></a>

<div class="space11"></div>

**변환되는 해상도**

1. Android
	* ldpi
	* mdpi
	* hdpi
	* xhdpi
	* xxhdpi
1. iOS
	* iPhone series
	* iPod series
	* iPad series

<div class="space33"></div>
<hr/>
<div class="space33"></div>
<div class="title row">
	업로드
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		이미지는 App 빌드 신청시에 규격에 맞춰 업로드 한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/splash_2.png" data-lightbox="splash_2" data-title="">
			<img src="/docs/images/splash_2.png" alt=""/>
		</a>
	</div>
</div>
