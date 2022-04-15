<script>

</script>


<svelte:head>
    <script src="https://www.google.com/recaptcha/api.js" async="" defer=""></script>
    <script type="text/javascript" src="https://s3.ap-northeast-2.amazonaws.com/resource.stibee.com/subscribe/stb_subscribe_form.js"></script>
</svelte:head>

<link rel="stylesheet" href="https://s3.ap-northeast-2.amazonaws.com/resource.stibee.com/subscribe/stb_subscribe_form_style.css">

<div id="stb_subscribe">
   <form action="https://stibee.com/api/v1.0/lists/yhxq5p-qeFAc5z19MILTHyeTaAfYGg==/public/subscribers" method="POST" target="_blank" accept-charset="utf-8" class="stb_form" name="stb_subscribe_form" id="stb_subscribe_form" novalidate="">
      <h1 class="stb_form_title">📧 쿠링 위클리 HOT 공지</h1>
      <p class="stb_form_description">매주 건국대학교를 뜨겁게 달군 공지사항들을 메일로 받아보세요. 장학금, 교환학생, 학사 일정 등 번거롭게 매번 건대 사이트에 접속할 필요가 더이상 없습니다. 정말 우리에게 필요한 소식만 깔끔하게 전달해드립니다!</p>
      <fieldset class="stb_form_set">
         <label for="stb_email" class="stb_form_set_label"> 이메일 주소<span class="stb_asterisk">*</span> </label> <input type="email" class="stb_form_set_input" id="stb_email" name="email" required="required"> 
         <div class="stb_form_msg_error" id="stb_email_error"></div>
      </fieldset>
      <div class="stb_form_policy">
         <label> <input type="checkbox" id="stb_policy" value="stb_policy_true"> <span>(필수)</span> <button id="stb_form_modal_open" data-modal="stb_form_policy_modal" class="stb_form_modal_open_btn" type="button">개인정보 수집 및 이용</button>에 동의합니다. </label> 
         <div class="stb_form_msg_error" id="stb_policy_error"></div>
         <div class="stb_form_modal stb_form_policy_text blind" id="stb_form_policy_modal">
            <div class="stb_form_modal_body">
               <h1 class="stb_form_modal_title"> 개인정보 수집 및 이용 </h1>
               <p class="stb_form_modal_text">뉴스레터 발송을 위한 최소한의 개인정보를 수집하고 이용합니다. 수집된 정보는 발송 외 다른 목적으로 이용되지 않으며, 서비스가 종료되거나 구독을 해지할 경우 즉시 파기됩니다.</p>
               <div class="stb_form_modal_btn"> <button id="stb_form_modal_close" class="stb_form_modal_close_btn" data-modal="stb_form_policy_modal" type="button">닫기</button> </div>
            </div>
            <div class="stb_form_modal_bg" id="stb_form_modal_bg"></div>
         </div>
      </div>
      <div class="stb_form_policy">
         <label> <input type="checkbox" id="stb_ad_agreement" value="stb_ad_agreement_true"> <span class="">(선택)</span> <button id="stb_form_ad_modal_open" data-modal="stb_form_ad_agreemnet_modal" class="stb_form_modal_open_btn" type="button">광고성 정보 수신</button>에 동의합니다. </label> 
         <div class="stb_form_msg_error" id="stb_ad_agreement_error"></div>
         <div class="stb_form_modal stb_form_policy_text blind" id="stb_form_ad_agreemnet_modal">
            <div class="stb_form_modal_body">
               <h1 class="stb_form_modal_title"> 광고성 정보 수신 </h1>
               <p class="stb_form_modal_text">제휴 콘텐츠, 프로모션, 이벤트 정보 등의 광고성 정보를 수신합니다.</p>
               <div class="stb_form_modal_btn"> <button id="stb_form_ad_modal_close" class="stb_form_modal_close_btn" data-modal="stb_form_ad_agreemnet_modal" type="button">닫기</button> </div>
            </div>
            <div class="stb_form_ad_modal_bg" id="stb_form_modal_bg"></div>
         </div>
      </div>
      <div class="stb_form_result" id="stb_form_result"> </div>
      <fieldset class="stb_form_set_submit"> <button type="submit" class="stb_form_submit_button" id="stb_form_submit_button" style="background-color: rgb(61, 189, 128); color: rgb(255, 255, 255);">구독하기</button> </fieldset>
   </form>
</div>
