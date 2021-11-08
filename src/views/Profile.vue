<template>
  <div >
    <b-container id="cont" class="main_con text-white pl-5 pt-5 text-left">
      <b-row class="pl-2 pr-2">
        <b-col cols="6" class="main_title">
          <!-- f5b895 f3d6ae 658dc6-->
          <h1  style="color:#F9F871;">#사이퍼즈 트친소</h1>
<!--          <b-img src="http://static.cyphers.co.kr/img/lnb/logo_new.png" alt="LOGO"/>-->
<!--          <b-icon stacked icon="slash-circle" variant="primary" style="width: 80px; height: 80px;"></b-icon>-->
        </b-col>
        <b-col cols="4" class="text-right" style="position: sticky;">
          <b-img thumbnail style="position: absolute; width: 300px; height: 300px; left:150px" src="https://placekitten.com/300/300" alt="프로필 사진"/>
        </b-col>
      </b-row>
      <b-row class="h-25 w-50">
        <b-col class="pt-3">
          <h1 class="profile_text" style="color:#959366;letter-spacing: -6px;">P R O F I L E</h1>
          <h1 class="mt-4" style="font-weight: 300">이룩 / 52급</h1>
          <h2 class="mt-4" style="font-weight: 300">CLAN 버텨보아라</h2>
<!--          <h6 class="mt-4" style="font-weight: 300">티어 클랜이름</h6>-->
        </b-col>
      </b-row>
      <b-row style="height: 50px"></b-row>
      <b-row class="h-25 pl-2 pr-2 mt-5">
        <b-col cols="3">
          <div>
            <p>
              <b-input-group>
                <template #prepend>
                  <b-icon-hexagon class="position_icon" style="width: 40px; height: 40px;"/>
                </template>
                <b-card-text style="font-size:24px;" class="pl-4">POSITION</b-card-text>
              </b-input-group>
            </p>
            <div class="d-flex feature_box">
              <b-card-text class="p-1 hashTag">
                # 탱커
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 원딜
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 근딜
              </b-card-text>
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 개발부-->
<!--              </b-card-text>-->
            </div>
          </div>
        </b-col>
        <b-col cols="3">
          <div>
            <p>
              <b-input-group>
                <template #prepend>
                  <b-icon-fullscreen style="width: 40px; height: 40px;"/>
                </template>
                <b-card-text style="font-size:24px;" class="pl-4">PLAY TYPE</b-card-text>
              </b-input-group>
            </p>
            <div class="d-flex feature_box">
              <b-card-text class="p-1 hashTag">
                # 일반
              </b-card-text>
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 개발부-->
<!--              </b-card-text>-->
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 개발부-->
<!--              </b-card-text>-->
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 개발부-->
<!--              </b-card-text>-->
            </div>
          </div>
<!--          <div class="pt-1">-->
<!--            <p>-->
<!--              <b-input-group>-->
<!--                <template #prepend>-->
<!--                  <b-icon-play style="width: 40px; height: 40px;"/>-->
<!--                </template>-->
<!--                <b-card-text style="font-size:24px;" class="pl-4">PLAY LIKE</b-card-text>-->
<!--              </b-input-group>-->
<!--            </p>-->
<!--            <div class="d-flex feature_box">-->
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 승지-->
<!--              </b-card-text>-->
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 조합-->
<!--              </b-card-text>-->
<!--              &lt;!&ndash;              <b-card-text class="p-1 hashTag">&ndash;&gt;-->
<!--              &lt;!&ndash;                # 개발부&ndash;&gt;-->
<!--              &lt;!&ndash;              </b-card-text>&ndash;&gt;-->
<!--              &lt;!&ndash;              <b-card-text class="p-1 hashTag">&ndash;&gt;-->
<!--              &lt;!&ndash;                # 개발부&ndash;&gt;-->
<!--              &lt;!&ndash;              </b-card-text>&ndash;&gt;-->
<!--              &lt;!&ndash;              <b-card-text class="p-1 hashTag">&ndash;&gt;-->
<!--              &lt;!&ndash;                # 개발부&ndash;&gt;-->
<!--              &lt;!&ndash;              </b-card-text>&ndash;&gt;-->
<!--            </div>-->
<!--          </div>-->
        </b-col>
        <b-col cols="3">
          <div>
            <p>
              <b-input-group>
                <template #prepend>
                  <b-icon-suit-heart style="width: 40px; height: 40px;"/>
                </template>
                <b-card-text style="font-size:24px;" class="pl-4">PLAY LIKE</b-card-text>
              </b-input-group>
            </p>
            <div class="d-flex feature_box">
              <b-card-text class="p-1 hashTag">
                # 승리지향
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 조합맞춤
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 즐거운분위기
              </b-card-text>
<!--              <b-card-text class="p-1 hashTag">-->

<!--              </b-card-text>-->
            </div>
          </div>
        </b-col>
        <b-col cols="3">
          <div>
            <p>
              <b-input-group>
                <template #prepend>
                  <b-icon-alarm style="width: 40px; height: 40px;"/>
                </template>
                <b-card-text style="font-size:24px;" class="pl-4">PLAY TIME</b-card-text>
              </b-input-group>
            </p>
            <div class="d-flex feature_box">
              <b-card-text class="p-1 hashTag">
                # 평일
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 주말
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 오후
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 새벽
              </b-card-text>
            </div>
          </div>
        </b-col>
      </b-row>
      <b-row class="h-25 pl-2 pr-2">
        <!--F type -->
        <b-col cols="3">
          <div>
            <p>
              <b-input-group>
                <template #prepend>
                  <b-icon-twitter style="width: 40px; height: 40px;"/>
                </template>
                <b-card-text style="font-size:24px;" class="pl-4">FOLLOW</b-card-text>
              </b-input-group>
            </p>
            <div class="d-flex feature_box">
              <b-card-text class="p-1 hashTag">
                # 마음
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 알티
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 멘션
              </b-card-text>
              <!--              <b-card-text class="p-1 hashTag">-->
              <!--                # 개발부-->
              <!--              </b-card-text>-->
            </div>
          </div>
        </b-col>
        <b-col cols="3">
          <div>
            <p>
              <b-input-group>
                <template #prepend>
                  <b-icon-people  style="width: 40px; height: 40px;"/>
                </template>
                <b-card-text style="font-size:24px;" class="pl-4">PARTY</b-card-text>
              </b-input-group>
            </p>
            <div class="d-flex feature_box">
              <!--              <b-card-text class="p-1 hashTag">-->
              <!--                # 솔플-->
              <!--                </b-card-text>-->
              <b-card-text class="p-1 hashTag">
                # 2인
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 3인
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 4인
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 5인
              </b-card-text>
            </div>
          </div>
        </b-col>
        <b-col cols="6">
          <div>
            <p>
              <b-input-group>
                <template #prepend>
                  <b-icon-journal style="color:#F9F871; width: 40px; height: 40px;"/>
                </template>
                <b-card-text style="font-size:24px; " class="pl-4">MEMO</b-card-text>
              </b-input-group>
            </p>
            <b-card-text class="pl-3 p-1 memo_box" style="border-left:3px dashed; word-break: break-all; ">
              안녕하세요 반갑습니다.
              해당 문항은 메모의 기능이며 글자수 제한을 체크해보려고 합니다.
              다른 문제 사항이 있다면 언제든 편히 말씀주세요
              감사합니다.
              안녕하세요 반갑습니다.
              해당 문항은 메모의 기능이며 글자수 제한을 체크해보려고 합니다.
              다른 문제 사항이 있다면 언제든
            </b-card-text>
<!--            <div class="d-flex feature_box">-->
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 2인-->
<!--              </b-card-text>-->
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 3인-->
<!--              </b-card-text>-->
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 4인-->
<!--              </b-card-text>-->
<!--              <b-card-text class="p-1 hashTag">-->
<!--                # 5인-->
<!--              </b-card-text>-->
<!--            </div>-->
          </div>
<!--          <b-card-text>-->
<!--          <form>-->
<!--            <fieldset style="border:1px solid" class="pl-3 pb-3">-->
<!--              <legend style="width: 100px;" class="memo_title"> MEMO</legend>-->
<!--                <b-card-text class="memo_box">-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->
<!--                  안녕하세요 반갑습니다.-->

<!--                </b-card-text>-->
<!--              </fieldset>-->
<!--            </form>-->
<!--          </b-card-text>-->
        </b-col>
      </b-row>
    </b-container>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <b-button @click="cap">capt</b-button>
    <canvas id="canvas" width="1024px" height="808px"></canvas>
  </div>

</template>

<script>
// import png from "@/assets/Discord-Logo-Color.png"
import html2canvas from "html2canvas";

export default {
  name: "Profile",
  methods:{
    cap(){
      html2canvas(document.querySelector('#cont'), { logging: true, letterRendering: 1, useCORS: true } ).then(function (canvas) {
        const link = document.createElement('a');
        link.href = canvas.toDataURL('image/png');
        link.download = 'test';
        document.body.appendChild(link);
        link.click();
      });
    },
    saveAs(uri, filename) {
      console.log(uri,filename)
    }
  }
}
</script>

<style scoped>
.main_con{
  height: 808px;
  width: 1024px;
  background: #141516;
  min-width: 1024px;
  max-width: 1024px;
}
.profile_text{
  font-size:40px;
}
h1{
  font-size: 48px;
  line-height: 58px;
  letter-spacing: -1px;
  clear: both;
  color: #fff;
  font-family: "Vitro_core", serif;
  font-weight: 600;
}
h2{
  color: #fff;
  font-family: "Vitro_core", serif;
  font-weight: 600;
}
.feature_box{
  flex-wrap: wrap;
  align-items: flex-start;

}
.input-group{
  font-family: "Vitro_core", serif;
}
.feature_box>.hashTag{
  /*border:1px solid #fff;*/
  /*border-radius: 20px;*/
  /*margin-right: 5px;*/
  font-weight: 500;
  margin:0;
  font-size:20px;
  letter-spacing: -1px;
  font-family: "Cafe24Oneprettynight",sans-serif;
}
.memo_title{
  font-weight: 400;
  font-size:40px;
  font-family: "Cafe24Oneprettynight",sans-serif;
}
.memo_box{
  font-weight: 400;
  font-size:16px;
  font-family: "MaruBuri-Regular",sans-serif;
}
.position_icon{
  background: linear-gradient(to right, #1865de, #d20e0c);
  border-radius: 17px;
  -webkit-text-fill-color: transparent;
}
/*타이틀*/
@font-face {
  font-family: 'Vitro_core';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_20-10-21@1.0/Vitro_core.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}

/*노트용*/
@font-face {
  font-family: 'HSYuji-Regular';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_2108@1.1/HSYuji-Regular.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}


@font-face {
  font-family: 'BMDOHYEON';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_one@1.0/BMDOHYEON.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}
@font-face {
  font-family: 'IBMPlexSansKR-Regular';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_20-07@1.0/IBMPlexSansKR-Regular.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}
/* 본문 */
@font-face {
  font-family: 'Cafe24Oneprettynight';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_twelve@1.1/Cafe24Oneprettynight.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}

@font-face {
  font-family: 'MaruBuri-Regular';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_20-10-21@1.0/MaruBuri-Regular.woff') format('woff');
  font-weight: normal;
  font-style: normal;
}
</style>
