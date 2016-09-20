---
title: certificate Issue & Integration
layout: docs
section: docs/distribute-cert
---

Certificate Issue & Integration
===================

이 문서에서는 앱을 빌드하고 배포하기 위한 인증서를 발급하고 appflush 전용 인증서인 appkey 파일을 발급하는 방법을 설명 합니다.

<hr/>
<div class="space33"></div>

#### 개발자 등록

1. Android
	- [Google Play 계정](https://play.google.com/apps/publish/signup/) (처음 1회 $25)
	- AppFlush에서 제작한 App을 빌드하여 배포 및 판매 하고자 할 경우 등록.
1. iOS
	- [Apple's Developer program 계정](//developer.apple.com/) (매년 1회 $99)
	- AppFlush에서 제작한 App을 빌드하여 배포 및 판매 하고자 할 경우 등록.
	- TheCore Preview 를 자신의 디바이스에 설치하고자 할 경우 등록.

> iOS는 TheCore Preview 설치를 위해서 Apple Developer program을 등록해 iOS 인증서를 받아야 합니다.<br/>

<div class="space11"></div>
<hr/>
<div class="space11"></div>

<div class="title row">
	Android 인증서 발급
</div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-4">
		<dl>
			<dt>Password</dt>
			<dd>패스워드</dd>
			<dt>Key alias</dt>
			<dd>키 식별 이름</dd>
			<dt>Common Name</dt>
			<dd>사용자/기관</dd>
			<dt>Organizational Unit</dt>
			<dd>부서</dd>
			<dt>Oranization</dt>
			<dd>회사</dd>
			<dt>City or Locality</dt>
			<dd>도시</dd>
			<dt>State or Province</dt>
			<dd>주</dd>
			<dt>Contry Code</dt>
			<dd>국가 코드</dd>
			<dt>validity day</dt>
			<dd>만료일 지정 최소 50년 이상</dd>
		</dl>
	</div>
	<div class="movie col-xs-12 col-md-8">
		<iframe class="thumbnail" id="ytplayer" type="text/html" width="100%" height="720"
src="https://www.youtube.com/embed/EOBvoI_Q4Aw?controls=1&enablejsapi=1&modestbranding=1&rel=0&showinfo=0&autohide=1&color=white&iv_load_policy=3&theme=light&vq=hd720"
frameborder="0" allowfullscreen></iframe>
	</div>
</div>

<div class="space33"></div>
<hr/>
<div class="space33"></div>

<div class="title row">
	iOS 인증서 발급
	<div class="space11"></div>
	<blockquote>
		<strong class="title_sub">발급 순서</strong>
		<ol class="title_sub">
			<li>Private Key 발급</li>
			<li>Certificate Signing Request 발급
				<ul style="font-weight:normal;">
					<li>private key 필요</li>
				</ul>
			</li>
			<li>iOS Certificate, APNS Certificate, WWDR Certificate, provisioning Profile
				<ul style="font-weight:normal;">
					<li>Apple Developer 에서 발급</li>
					<li>Certificate Signing Request 필요</li>
				</ul>
			</li>
			<li>AppKey 발급
				<ul style="font-weight:normal;">
					<li><a href="#private">Private Key</a></li>
					<li><a href="#csr">Certificate Signing Request</a></li>
					<li><a href="#cert">iOS Certificate</a></li>
					<li><a href="#apns">APNS Certificate</a></li>
					<li><a href="#wwdr">WWDR Certificate</a></li>
					<li><a href="#prov">provisioning Profile 필요</a></li>
				</ul>
			</li>
		 </ol>
	</blockquote>
</div>
<hr id="private"/>
<div class="space33"></div>
<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>Private Key 발급</strong>
		<div class="space11"></div>
		발급된 Private Key는 서버에 저장되지 않는다.<br/>
		Private Key는 인증서, CSR, 프로비저닝 파일등을 생성하기 위해 필요한 파일로, 분실되지 않도록 안전한 곳에 백업해 놓는 것이 좋다.
		<div class="space11"></div>
		인증서 관리 > private Key 발급 페이지에서 발급 받을 수 있다.
		<div class="space11"></div>
		OSX상에서 생성한 키가 있다면 PKCS12 포맷으로 추출해 Private Key를 대신할 수 있다. <a href="/docs/distribute-p12.html">[자세히 보기]</a>
	</div>
	<div class="movie col-xs-12 col-md-6">

		<a class="thumbnail" data-toggle="lightbox" href="#ios_private_1"><img src="/docs/images/ios_private_1.png" alt=""/></a>
		<div id="ios_private_1" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/ios_private_1.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#ios_private_2"><img src="/docs/images/ios_private_2.png" alt=""/></a>
		<div id="ios_private_2" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/ios_private_2.png" alt=""/>
				  </div>
			 </div>
		</div>
	</div>
</div>

<div class="space33"></div>
<hr id="csr"/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>CSR (Certificate Signing Request) 발급</strong>
		<div class="space11"></div>
		발급된 CSR파일은 서버에 저장되지 않습니다.<br/>
		CSR 파일은 인증서, 프로비저닝 파일등을 생성하기 위해 필요한 파일<br/>
		<div class="space11"></div>
		인증서 관리 > CSR 발급 페이지에서 발급 받을 수 있다.
		<div class="space11"></div>
		위에서 발급한 Private Key 파일이 필요 하다.
	</div>
	<div class="movie col-xs-12 col-md-6">

		<a class="thumbnail" data-toggle="lightbox" href="#ios_CSR_1"><img src="/docs/images/ios_CSR_1.png" alt=""/></a>
		<div id="ios_CSR_1" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/ios_CSR_1.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#ios_CSR_2"><img src="/docs/images/ios_CSR_2.png" alt=""/></a>
		<div id="ios_CSR_2" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/ios_CSR_2.png" alt=""/>
				  </div>
			 </div>
		</div>
	</div>
</div>


<div class="space33"></div>
<hr id="cert"/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>iOS 인증서 발급</strong>
		<div class="space11"></div>
		위에서 발급한 CSR 파일이 필요 하다.
	</div>
	<div class="movie col-xs-12 col-md-6">

		<a class="thumbnail" data-toggle="lightbox" href="#apple_login"><img src="/docs/images/apple_login.png" alt=""/></a>
		<div id="apple_login" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/apple_login.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#cert_1"><img src="/docs/images/cert_1.png" alt=""/></a>
		<div id="cert_1" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/cert_1.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#cert_2"><img src="/docs/images/cert_2.png" alt=""/></a>
		<div id="cert_2" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/cert_2.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#cert_3"><img src="/docs/images/cert_3.png" alt=""/></a>
		<div id="cert_3" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/cert_3.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#cert_4"><img src="/docs/images/cert_4.png" alt=""/></a>
		<div id="cert_4" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/cert_4.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#cert_5"><img src="/docs/images/cert_5.png" alt=""/></a>
		<div id="cert_5" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/cert_5.png" alt=""/>
				  </div>
			 </div>
		</div>
	</div>
</div>


<div class="space33"></div>
<hr id="apns"/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>APNS 인증서 발급</strong>
		<div class="space11"></div>
		위에서 발급한 CSR 파일이 필요 하다.
	</div>
	<div class="movie col-xs-12 col-md-6">

		<a class="thumbnail" data-toggle="lightbox" href="#apns_1"><img src="/docs/images/cert_2.png" alt=""/></a>
		<div id="apns_1" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/cert_2.png" alt=""/>
				  </div>
			 </div>
		</div>

		<a class="thumbnail" data-toggle="lightbox" href="#apns_2"><img src="/docs/images/apns_1.png" alt=""/></a>
		<div id="apns_2" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/apns_1.png" alt=""/>
				  </div>
			 </div>
		</div>
	</div>
</div>

<div class="space33"></div>
<hr id="wwdr"/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>WWDR 인증서 발급</strong>
		<div class="space11"></div>
	</div>
	<div class="movie col-xs-12 col-md-6">

		<a class="thumbnail" data-toggle="lightbox" href="#wwdr_1"><img src="/docs/images/cert_2.png" alt=""/></a>
		<div id="wwdr_1" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/cert_2.png" alt=""/>
				  </div>
			 </div>
		</div>

		<a class="thumbnail" data-toggle="lightbox" href="#wwdr_2"><img src="/docs/images/wwdr_1.png" alt=""/></a>
		<div id="wwdr_2" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/wwdr_1.png" alt=""/>
				  </div>
			 </div>
		</div>
	</div>
</div>

<div class="space33"></div>
<hr id="appid"/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>App ID 생성</strong>
		<div class="space11"></div>
		App ID는 AppFlush 에서 Project 생성시 입력한 App ID와 같다.
	</div>
	<div class="movie col-xs-12 col-md-6">

		<a class="thumbnail" data-toggle="lightbox" href="#appid_1"><img src="/docs/images/appid_1.png" alt=""/></a>
		<div id="appid_1" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/appid_1.png" alt=""/>
				  </div>
			 </div>
		</div>

		<a class="thumbnail" data-toggle="lightbox" href="#appid_2"><img src="/docs/images/appid_2.png" alt=""/></a>
		<div id="appid_2" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/appid_2.png" alt=""/>
				  </div>
			 </div>
		</div>

		<a class="thumbnail" data-toggle="lightbox" href="#appid_3"><img src="/docs/images/appid_3.png" alt=""/></a>
		<div id="appid_3" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/appid_3.png" alt=""/>
				  </div>
			 </div>
		</div>
	</div>
</div>

<div class="space33"></div>
<hr id="appid"/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>Ad-hoc Device 등록</strong>
		<div class="space11"></div>
		Adhoc은 앱을 배포하기 전에 디바이스에 개발중인 앱을 설치해 볼 수 있는 기능으로 최대 100대까지 등록이 가능하다. TheCore Preview를 설치하기 위해서는 ad-hoc Provisioning이 필요하다. 여기에서 미리 디바이스를 등록한다.
		<div class="space11"></div>
		<strong>UUID</strong><br/>
		UUID는 기기 고유 아이디 이며 아이튠즈에서 디바이스를 연결 한 후 확인 할 수 있다.
	</div>
	<div class="movie col-xs-12 col-md-6">

		<a class="thumbnail" data-toggle="lightbox" href="#device_1"><img src="/docs/images/device_1.png" alt=""/></a>
		<div id="device_1" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/device_1.png" alt=""/>
				  </div>
			 </div>
		</div>

		<a class="thumbnail" data-toggle="lightbox" href="#device_2"><img src="/docs/images/device_2.png" alt=""/></a>
		<div id="device_2" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/device_2.png" alt=""/>
				  </div>
			 </div>
		</div>

		<a class="thumbnail" data-toggle="lightbox" href="#device_3"><img src="/docs/images/device_3.png" alt=""/></a>
		<div id="device_3" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/device_3.png" alt=""/>
				  </div>
			 </div>
		</div>
	</div>
</div>

<div class="space33"></div>
<hr id="prov"/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-6">
		<strong>Provisioning Profile 생성</strong>
		<div class="space11"></div>
		App ID는 AppFlush 에서 Project 생성시 입력한 App ID와 같다.
		<div class="space11"></div>
		<strong>App Store</strong><br/>
		앱스토어 배포 전용으로 앱스토어 업로드시에 사용한다.
		<div class="space11"></div>
		<strong>Ad Hoc</strong><br/>
		디바이스 테스트용으로 등록된 디바이스에 한해 설치 할 수 있다. TheCore Preview App은 이 인증서를 이용해 빌드 해야 한다.
	</div>
	<div class="movie col-xs-12 col-md-6">

		<a class="thumbnail" data-toggle="lightbox" href="#prov_1"><img src="/docs/images/prov_1.png" alt=""/></a>
		<div id="prov_1" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/prov_1.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#prov_2"><img src="/docs/images/prov_2.png" alt=""/></a>
		<div id="prov_2" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/prov_2.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#prov_3"><img src="/docs/images/prov_3.png" alt=""/></a>
		<div id="prov_3" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/prov_3.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#prov_4"><img src="/docs/images/prov_4.png" alt=""/></a>
		<div id="prov_4" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/prov_4.png" alt=""/>
				  </div>
			 </div>
		</div>
<a class="thumbnail" data-toggle="lightbox" href="#prov_4_1"><img src="/docs/images/prov_4_1.png" alt=""/></a>
		<div id="prov_4_1" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/prov_4_1.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#prov_5"><img src="/docs/images/prov_5.png" alt=""/></a>
		<div id="prov_5" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/prov_5.png" alt=""/>
				  </div>
			 </div>
		</div>
		<a class="thumbnail" data-toggle="lightbox" href="#prov_6"><img src="/docs/images/prov_6.png" alt=""/></a>
		<div id="prov_6" class="lightbox fade"  tabindex="-1" role="dialog" aria-hidden="true">
			 <div class='lightbox-dialog'>
				  <div class='lightbox-content'>
						<img src="/docs/images/prov_6.png" alt=""/>
				  </div>
			 </div>
		</div>
	</div>
</div>

<div class="space33"></div>
<hr id="appkey"/>
<div class="space33"></div>

<div class="explain row">
	<div class="detail col-xs-12 col-md-4">
		<strong>appkey 발급</strong>
		<div class="space11"></div>
		appkey는 여러 인증서 파일을 AppFlush에서 편리하게 사용하기 위한 전용 통합 키 파일.
		<div class="space11"></div>
		<dl>
			<dt>Private Key</dt>
			<dd>AppFlush에서 발급한 Private Key</dd>
			<dt>iOS Certificate</dt>
			<dd>Apple Developer program에서 발급한 개발자 인증서</dd>
			<dt>APNS Certificate</dt>
			<dd>Apple Developer program에서 발급한 APNS 인증서</dd>
			<dt>WWDR Certificate</dt>
			<dd>Apple Developer program에서 발급한 WWDR 인증서</dd>
			<dt>provisioning Profile</dt>
			<dd>Apple Developer program에서 발급한 provisioning 파일</dd>
			<dt>AppKey Password</dt>
			<dd>AppKey를 사용하기 위한 패스워드</dd>
		</dl>
	</div>
	<div class="movie col-xs-12 col-md-8">
		<iframe class="thumbnail" id="ytplayer" type="text/html" width="100%" height="720"
src="https://www.youtube.com/embed/h9sbBAM6w1A?controls=1&enablejsapi=1&modestbranding=1&rel=0&showinfo=0&autohide=1&color=white&iv_load_policy=3&theme=light&vq=hd720"
frameborder="0" allowfullscreen></iframe>
	</div>
</div>

<div class="space33"></div>
<hr/>
<div class="space33"></div>
