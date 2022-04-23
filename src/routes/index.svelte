<div class="paper-container">
    <ImageList class="my-image-list-standard">
        {#each bannerImages as image}
            <Item>
                <ImageAspectContainer>
                    <Image
                        src={image.src}
                        alt={image.alt}
                    />
                </ImageAspectContainer>
            </Item>
        {/each}
    </ImageList>

    <h1>👋 쿠링에 오신 것을 환영합니다.</h1>
    <p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

    <Paper color="primary" variant="outlined">
        <Title>🔔 쿠링 - 건국대학교 공지앱</Title>

        <Subtitle style="position:relative">
            <span style="position:relative">
                건국대학교 공지사항을 알림으로 받아보세요!
                <Badge aria-label="unread count">3</Badge>
            </span>
        </Subtitle>

        <Content>
            <Button color="primary" on:click={openAppDownloadLink} variant="outlined">
                <Label>앱 다운로드</Label>
            </Button>
        </Content>
    </Paper>

    <Paper color="primary" variant="outlined">
        <Title>
            <span style="position: relative; display: inline-block; padding: .2em;">
                📰 쿠링 위클리 HOT 공지
                <Badge color="secondary" aria-label="unread count">beta</Badge>
            </span>
        </Title>

        <Subtitle style="position:relative">
            <span style="position:relative">
                매주 건국대학교 주요 공지를 간단하게 메일로 받아보세요.
            </span>
        </Subtitle>

        <Content>
            <p>
                장학금, 교환학생, 학사 일정 등 번거롭게 매번 건대 사이트에 접속할 필요가 더이상 없습니다. 
                정말 우리에게 필요한 소식만 깔끔하게 전달해드립니다!
            </p>
            <Button color="primary" on:click={openEmailSubscription} variant="outlined">
                <Label>이메일 구독하기</Label>
                <Badge color="secondary" aria-label="unread count">beta</Badge>
            </Button>
        </Content>
    </Paper>
</div>
 
<script lang="ts">
    import Badge from '@smui-extra/badge';
    import Button, { Label } from '@smui/button';
    import Paper, { Title, Subtitle, Content } from '@smui/paper';
    import ImageList, { Item, ImageAspectContainer, Image } from '@smui/image-list';

    let bannerImages = [
        { alt: "쿠링이미지01", src: "https://user-images.githubusercontent.com/53814741/163469327-98af5c02-efc7-4c3e-8fec-9195ca6805ad.JPG" },
        { alt: "쿠링이미지02", src: "https://user-images.githubusercontent.com/53814741/163469357-aed6a78a-4b65-4a9a-bead-d541e7eee702.JPG" },
        { alt: "쿠링이미지03", src: "https://user-images.githubusercontent.com/53814741/163469345-503b6b50-b240-4c8d-9656-c719a5f3d9f2.JPG" },
    ];

    function openAppDownloadLink() {
        window.open("https://ku-ring.onelink.me/Yxhp/ba3d81ce");
    }		

    function openEmailSubscription() {
        window.open("https://page.stibee.com/subscriptions/177667");
    }
</script>

<style>
    * :global(.paper-container) {
    padding: 24px;
    background-color: var(--mdc-theme-background, #f8f8f8);
  }
  * :global(.smui-paper) {
    margin: 0 auto 24px;
    max-width: 800px;
  }
  * :global(.smui-paper:last-child) {
    margin-bottom: 0;
  }
</style>