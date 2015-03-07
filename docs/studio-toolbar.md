---
title: App Studio - Toolbar
layout: docs
section: docs/studio-toolbar
---

App Studio - Toolbar
===================

이 문서에서는 App Studo의 Toolbar에 대해서 설명 합니다.

툴바는 App Studio에서 여러 프로젝트에서 공통으로 사용되는 기능을 모아 놓은 기능들의 모음 입니다.

<hr/>
<div class="space33"></div>

<div class="title row">
	Studio 툴바
</div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<dl>
			<dt>Project Type</dt>
			<dd>현재 프로젝트의 종류</dd>
			<dt>Connect</dt>
			<dd>실시간 통신을 위한 서버 연결 및 해제</dd>
			<dt>Module</dt>
			<dd>글로벌 아이템 영역에 commonJS 모듈을 추가</dd>
			<dt>Script</dt>
			<dd>글로벌 아이템 영역에 Javascript를 직접 입력 할 수 있는 스크립트 추가</dd>
			<dt>Refresh</dt>
			<dd>현재 작업 영역과 연결된 디바이스들을 다시 로드 한다.</dd>
			<dt>Fit Screen</dt>
			<dd>연결된 디바이스 중 선택된 디바이스의 화면의 크기와 작업 영역의 크기 동기화, 여러대의 디바이스가 연결된 경우 기준이 되는 디바이스를 선택 할 수 있다.</dd>
			<dt>휴지통</dt>
			<dd>드랍 된 아이템을 화면 및 메모리에서 제거</dd>
			<dt>TiApp</dt>
			<dd>필요한 경우 Titanium 설정 추가</dd>
			<dt>Maps</dt>
			<dd>지역명으로 지도의 경도, 위도 값 검색</dd>
			<dt>Storage</dt>
			<dd>파일 및 미디어 저장 공간</dd>
			<dt>Build</dt>
			<dd>현재 프로젝트를 설치 및 배포 가능한 App으로 빌드</dd>
		</dl>
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar.jpg" data-lightbox="studio_toolbar" data-title="">
			<img src="/docs/images/studio_toolbar.jpg" alt=""/>
		</a>
	</div>
</div>

<div class="space11"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	프로젝트 종류
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		현재 프로젝트의 플랫폼 종류를 단순 표시한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_type.png" data-lightbox="studio_toolbar_type" data-title="type">
			<img src="/docs/images/studio_toolbar_type.png" alt="type"/>
		</a>
	</div>
</div>
<div class="space33"></div>
<div class="title row">
	서버 연결
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		프로젝트를 편집하기 위해 서버에 연결하거나 종료한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_connect.png" data-lightbox="studio_toolbar_connect" data-title="connect">
			<img src="/docs/images/studio_toolbar_connect.png" alt="connect"/>
		</a>
	</div>
</div>
<div class="space33"></div>
<div class="title row">
	모듈, 스크립트
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		글로벌 아이템 영역에 모듈(commonJS), 스크립트(Titanium Script) 아이템을 생성한다. 직접 스크립트를 이용해 App을 제작할 수 있다. <small><a href="/docs/studio-script.html">[자세히보기]</a></small>
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_script_module.png" data-lightbox="studio_toolbar_script_module" data-title="module">
			<img src="/docs/images/studio_toolbar_script_module.png" alt="module"/>
		</a>
		<a class="thumbnail" href="/docs/images/studio_toolbar_script_module_preview.png" data-lightbox="studio_toolbar_script_module_preview" data-title="module">
			<img src="/docs/images/studio_toolbar_script_module_preview.png" alt="module"/>
		</a>
	</div>
</div>
<div class="space33"></div>
<div class="title row">
	새로고침
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		현재 수정되고 있는 글로벌 아이템을 서버에 저장된 데이타로 다시 화면에 표시한다. 동시에 디바이스에 전송해 디바이스에도 함께 표시한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_refresh.png" data-lightbox="studio_toolbar_refresh" data-title="refresh">
			<img src="/docs/images/studio_toolbar_refresh.png" alt="refresh"/>
		</a>
	</div>
</div>
<div class="space33"></div>
<div class="title row">
	화면 맞춤
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		연결되어 있는 디바이스에 화면 크기를 가져와 App Studio의 작업창의 크기에 적용한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_fitscreen.png" data-lightbox="studio_toolbar_fitscreen" data-title="fitscreen">
			<img src="/docs/images/studio_toolbar_fitscreen.png" alt="fitscreen"/>
		</a>
		<a class="thumbnail" href="/docs/images/studio_toolbar_fitscreen_preview.png" data-lightbox="studio_toolbar_fitscreen_preview" data-title="fitscreen">
			<img src="/docs/images/studio_toolbar_fitscreen_preview.png" alt="fitscreen"/>
		</a>
	</div>
</div>
<div class="space33"></div>
<div class="title row">
	휴지통
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		드랍된 아이템을 서버에서 영구 제거한다. 디바이스에도 적용되어 아이템이 삭제 된다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_trash.png" data-lightbox="studio_toolbar_trash" data-title="trash">
			<img src="/docs/images/studio_toolbar_trash.png" alt="trash"/>
		</a>
	</div>
</div>
<div class="space33"></div>
<div class="title row">
	TiApp.xml
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		배포용 App을 빌드할때 추가적인 빌드 옵션을 추가 한다. App에 추가적인 권한이나 정보를 저장할 필요가 있을 경우 사용된다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_tiapp.png" data-lightbox="studio_toolbar_tiapp" data-title="tiapp">
			<img src="/docs/images/studio_toolbar_tiapp.png" alt="tiapp"/>
		</a>
		<a class="thumbnail" href="/docs/images/studio_toolbar_tiapp_preview.png" data-lightbox="studio_toolbar_tiapp_preview" data-title="tiapp">
			<img src="/docs/images/studio_toolbar_tiapp_preview.png" alt="tiapp"/>
		</a>
	</div>
</div>
<div class="space33"></div>
<div class="title row">
	맵
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		주소를 이용 MapView에서 사용하는 좌표를 구하기 위해 사용한다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_map.png" data-lightbox="studio_toolbar_map" data-title="maps">
			<img src="/docs/images/studio_toolbar_map.png" alt="maps"/>
		</a>
		<a class="thumbnail" href="/docs/images/studio_toolbar_map_preview.png" data-lightbox="studio_toolbar_map_preview" data-title="maps">
			<img src="/docs/images/studio_toolbar_map_preview.png" alt="maps"/>
		</a>
	</div>
</div>
<div class="space33"></div>
<div class="title row">
	개인 저장소
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		App Studio에 이미지, 미디어 파일등을 저장하고 디바이스와 연동해 사용할 수 있는 개인 저장소이다. App Studio 액션창과 연동되어 편리하게 온라인 주소를 디바이스에 적용할 수 있다.
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_storage.png" data-lightbox="studio_toolbar_storage" data-title="storage">
			<img src="/docs/images/studio_toolbar_storage.png" alt="storage"/>
		</a>
		<a class="thumbnail" href="/docs/images/studio_toolbar_storage_preview.png" data-lightbox="studio_toolbar_storage_preview" data-title="storage">
			<img src="/docs/images/studio_toolbar_storage_preview.png" alt="storage"/>
		</a>
		<a class="thumbnail" href="/docs/images/studio_toolbar_storage_preview2.png" data-lightbox="studio_toolbar_storage_preview2" data-title="storage">
			<img src="/docs/images/studio_toolbar_storage_preview2.png" alt="storage"/>
		</a>
	</div>
</div>
<div class="space33"></div>
<div class="title row">
	빌드(컴파일)
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		현재 프로젝트를 디바이스에 설치 가능한 형태로 빌드(컴파일) 하기 위한 기능
	</div>
	<div class="movie col-xs-12 col-md-6">
		<a class="thumbnail" href="/docs/images/studio_toolbar_build.png" data-lightbox="studio_toolbar_build" data-title="build">
			<img src="/docs/images/studio_toolbar_build.png" alt="build"/>
		</a>
	</div>
</div>
<div class="space33"></div>
