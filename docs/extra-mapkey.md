---
title: Google API Key
layout: docs
section: docs/extra-mapkey
---

Google API Key
===================

AppFlush의 MapView 아이템은 Android의 Google Maps v2 모듈을 사용합니다. 구글 맵을 이용하기 위해서는 구글 API 콘솔에서 Google Maps API key를 발급 받아야 합니다.

1. 구글 API 프로젝트를 생성 합니다. <a href="https://developers.google.com/maps/documentation/android/start#create_an_api_project_in_the_google_apis_console" target="_blank">[Create an API project in the Google APIs Console]</a>
1. Google Maps API를 생성해 프로젝트 수정 페이지에 입력 합니다. <a href="https://developers.google.com/maps/documentation/android/start#obtain_a_google_maps_api_key" target="_blank">[Obtain a Google Maps API key]</a>.
	- Google Maps API key를 생성하기 위해서 App 프로젝트 각각 발급 받아야 합니다.
	- 프로젝트 AppID 와 키스토어의 SHA-1 certificate fingerprint가 요구 됩니다.

<div class="space11"></div>

<strong>구글 맵 키 발급</strong>

1. 구글 API 콘솔에 접속 합니다. <a href="https://code.google.com/apis/console/?noredirect" target="_blank">[Google APIs Console]</a>
1. **Services** 페이지에서, "Google Maps Android API v2" 가 활성화 되어 있는지 확인 합니다.
1. 네비게이션 메뉴에서 **API Access** 를 클릭 합니다.
1. **Create New Android Key...** 를 클릭 합니다.
1. 팝업창에 SHA-1 fingerprint를 입력하고 세미콜론을 붙인 후 App ID를 입력 합니다.
	- BB:0D:AC:74:D3:21:E1:43:67:71:9B:62:91:AF:A1:66:6E:44:5D:75;com.example.android.mapexample
1. 발급된 Google API 키를 확인 합니다.
	- AIzaSyBdVl-cTICSwYKrZ95SuvNw7dbMuDt1KG0

> <a href="https://www.youtube.com/results?search_query=How+to+get+the+Google+Maps+API+key" target="_blank">[Google Maps API Key 유투브 검색]</a>

<div class="space11"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	SHA-1 확인
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		Android의 인증서 생성시 함께 생성된 keyInfo.txt 파일내에 SHA-1 값이 포함되어 있다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/extra_mapkey_sha1.png" data-lightbox="extra_mapkey_sha1" data-title="">
			<img src="/docs/images/extra_mapkey_sha1.png" alt=""/>
		</a>
	</div>
</div>

<div class="space11"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	MapKey 입력
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		프로젝트 빌드 전에 수정 페이지로 이동해 MapKey를 입력한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/extra_mapkey_mapkey.png" data-lightbox="extra_mapkey_mapkey" data-title="">
			<img src="/docs/images/extra_mapkey_mapkey.png" alt=""/>
		</a>
	</div>
</div>