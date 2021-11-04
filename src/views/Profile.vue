<template>
  <div >
    <b-container class="main_con text-white pl-5 pt-5 text-left">
      <b-row class="pl-2 pr-2">
        <b-col cols="2">
          <b-icon stacked icon="slash-circle" variant="primary" style="width: 100px; height: 100px;"></b-icon>
        </b-col>
        <b-col cols="5" class="text-right" style="position: sticky;">
          <b-img style="position: absolute;" thumbnail src="https://placekitten.com/300/300" alt="프로필 사진"/>
        </b-col>
      </b-row>
      <b-row class="h-25 w-50">
        <b-col class="pt-3">
          <h1 style="letter-spacing: -6px;">P R O F I L E</h1>
          <h3 class="mt-4" style="font-weight: 300">이름</h3>
        </b-col>
      </b-row>
      <b-row style="height: 50px"></b-row>
      <b-row class="h-25 pl-2 pr-2 mt-5">
        <b-col cols="3" v-for="i in 4" :key="i+'fe'">
          <div>
            <p>
              <b-input-group>
                <template #prepend>
                  <b-icon-card-checklist variant="primary" style="width: 40px; height: 40px;"/>
                </template>
                <b-card-text style="font-size:26px;" class="pl-4">소속</b-card-text>
              </b-input-group>
            </p>
            <div class="d-flex feature_box">
              <b-card-text class="p-1 hashTag">
                # 개발부
                </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 개발부
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 개발부
                </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 개발부
              </b-card-text>
            </div>
          </div>
        </b-col>
      </b-row>
      <b-row class="h-25 pl-2 pr-2">
        <b-col cols="3" v-for="i in 2" :key="i+'fe'">
          <div>
            <p>
              <b-input-group>
                <template #prepend>
                  <b-icon-card-checklist variant="primary" style="width: 40px; height: 40px;"/>
                </template>
                <b-card-text style="font-size:26px;" class="pl-4">소속</b-card-text>
              </b-input-group>
            </p>
            <div class="d-flex feature_box">
              <b-card-text class="p-1 hashTag">
                # 개발부
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 개발부
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 개발부
              </b-card-text>
              <b-card-text class="p-1 hashTag">
                # 개발부
              </b-card-text>
            </div>
          </div>
        </b-col>
        <b-col cols="6">
          <b-card-text>
          <form>
            <fieldset style="border:1px solid" class="pl-3">
              <legend style="width: 100px;"> MEMO</legend>
                <b-card-text>
                  안녕하세요 반갑습니다.

                </b-card-text>
                <br>
              </fieldset>
            </form>
          </b-card-text>
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
  </div>

</template>

<script>
export default {
  name: "Profile"
}
</script>

<style scoped>
.main_con{
  height: 808px;
  width: 1024px;
  background: #141516;
}
h1{
  font-size: 48px;
  line-height: 58px;
  letter-spacing: -1px;
  clear: both;
  color: #fff;
  font-family: "Titillium Web", sans-serif;
  font-weight: 600;
}
.feature_box{
  flex-wrap: wrap;
  align-items: flex-start;
}
.feature_box>.hashTag{
  border:1px solid #fff;
  border-radius: 20px;
  margin-right: 5px;
  font-weight: 500;
  letter-spacing: -1px;
}
</style>
