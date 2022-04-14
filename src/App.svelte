<script lang="ts">
	let title = "🎉 쿠링에 오신 것을 환영합니다.";
	let serviceKuring = {
		  title: "쿠링 - 건국대학교 공지앱",
			eng: "KU Ring - KU Announcements app",
			description: "건국대학교 공지사항, 매번 학교홈페이지 들어가지 말고 이제 알림으로 받아보세요. 원하는 공지 카테고리를 구독하고 새 공지가 올라오면 곧바로 푸시 알림으로 받을 수 있습니다.",
			link: "https://ku-ring.onelink.me/Yxhp/ba3d81ce"
	}
	let serviceKUWeeklyHot = {
			title: "건대 위클리 HOT 공지",
			eng: "KU Weekly HOT Announcemnts",
			description: "매주 건국대학교를 뜨겁게 달군 공지사항들을 메일로 받아보세요. 장학금, 교환학생, 학사 일정 등 번거롭게 매번 건대 사이트에 접속할 필요가 더이상 없습니다. 정말 우리에게 필요한 소식만 깔끔하게 전달해드립니다!",
			link: "https://page.stibee.com/subscriptions/176230"
	}
	
	function openAppDownload() {
		window.open(serviceKuring.link)
	}
	
	function openEmailSubscription() {
		window.open(serviceKUWeeklyHot.link)
	}
</script>

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">

<main>
	<div class="d-flex align-items-start flex-column bd-highlight mb-3">
		<div class="mb-auto p-2 bd-highlight">
			
			<img alt="쿠링이미지01" src="https://user-images.githubusercontent.com/53814741/163469327-98af5c02-efc7-4c3e-8fec-9195ca6805ad.JPG" width=32%>
			<img alt="쿠링이미지02" src="https://user-images.githubusercontent.com/53814741/163469357-aed6a78a-4b65-4a9a-bead-d541e7eee702.JPG" width=32%>
			<img alt="쿠링이미지02" src="https://user-images.githubusercontent.com/53814741/163469345-503b6b50-b240-4c8d-9656-c719a5f3d9f2.JPG" width=32%>
			
			<!-- 쿠링 앱 -->
			
			<p class="fs-1 fw-bold">
				{title}
			</p>
			
			<p class="fs-3 fw-bold">
				{serviceKuring.title}
			</p>
			
			<p class="fw-normal">
				{serviceKuring.description}
			</p>
			
			<button type="button" class="btn btn-outline-success mb-5" on:click={openAppDownload}>
				앱 다운로드 받기
			</button>
			
			<!-- 쿠링 위클리 핫 공지 -->
			
			<p class="fs-3 fw-bold">
				{serviceKUWeeklyHot.title}
			</p>

			<p>
				{serviceKUWeeklyHot.description}
			</p>
			
			
			<button type="button" class="btn btn-outline-success disabled" on:click={openEmailSubscription}>
				이메일 구독하기 (서비스 준비중)
			</button>
		</div>
	</div>
</main>

<style>
	main {
		text-align: left;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>