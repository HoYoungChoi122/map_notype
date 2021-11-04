<template>
  <div >
    <b-form-file
        v-model="file1"
        :state="Boolean(file1)"
        @change="viewFile"
        placeholder="Choose a file or drop it here..."
        drop-placeholder="Drop file here..."
    ></b-form-file>
    <b-button @click="viewFile">파일 확인</b-button>
/*    <img class="popupImageItem"  alt="이미지업로드" style="width: 300px; height: 300px;">*/
    <b-img thumbnail fluid :src="uploadImageFile" alt="Image 1" style="width: 300px; height: 300px;"></b-img>
    <br>
    <div class="container">
      <b-table-simple >
        <b-thead>
          <b-th v-for="i in 12" :key="i">TH</b-th>
        </b-thead>
        <b-tbody>
          <b-td v-for="i in 12" :key="i">td</b-td>
        </b-tbody>

      </b-table-simple>
    </div>
    <b-container fluid class="p-4 container main_con">
      <b-row>
        <b-col>
          <b-row>
            <b-col cols="4">
              <b-img thumbnail class="thumbnail_img"  src="https://placekitten.com/300/300" alt="프로필 사진"/>
            </b-col>
            <b-col cols="8">

              <b-row class="info_table">
                <b-col cols="6" class="p-2">
                  <label class="m-0 label_con w-100 p-1">
                    <label class="tag_title">이름</label> <label class="tag_detail">ㅠㅠㅠ</label>
                  </label>
                </b-col>
                <b-col cols="6" class="p-2">
                  <label class="m-0 label_con w-100 p-1">
                    <label class="tag_title">회사</label> <label class="tag_detail">ㅇㅇㅇ</label>
                  </label>
                </b-col>

              </b-row>

              <b-row class="info_table">
                <b-col v-for="i in 12" :key="i">dd</b-col>
              </b-row>
            </b-col>
          </b-row>

        </b-col>
      </b-row>



    </b-container>
    <br>
    <br>
    <br>
    <b-container>
      <div class="cards">
        <div class="card content">
          <div class="card-content">
            <div class="card-img">
              <img src="https://images.unsplash.com/photo-1542751371-adc38448a05e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2850&q=80" alt="Gamer">
            </div>
            <div class="card-label">E-Sports</div>
            <div class="card-title">
              Fnatic raises $19 million, shakes up leadership team
            </div>
          </div>
        </div>
        <div class="card content">
          <div class="card-content">
            <div class="card-img">
              <img src="https://images.unsplash.com/photo-1547394765-185e1e68f34e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1950&q=80" alt="keyboard">
            </div>
            <div class="card-label">
              Technology
            </div>
            <div class="card-title">
              Google Stadia: The Future of Gaming
            </div>
          </div>
        </div>
        <div class="card content">
          <div class="card-content">
            <div class="card-img">
              <img src="https://images.unsplash.com/photo-1519326844852-704caea5679e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2034&q=80" alt="Controller">
            </div>
            <div class="card-label">
              Consoles
            </div>
            <div class="card-title">
              PS5 won't launch before mid-2020
            </div>
          </div>
        </div>
        <div class="card form">
          <div class="form-title" ref="test">ㅅㄷㄴㅅ</div>
        </div>
      </div>
    </b-container>

  </div>
</template>

<script>
export default {
  name: "ImageFile",
  data : ()=> ({
    file1 : null,
    uploadImageFile:'',

  }),
  methods : {
    viewFile(){
      console.dir(this.$refs.test.style)
      const file = this.file1
      if(file){
        const reader = new FileReader();

        reader.onload = (e) => {
          this.uploadImageFile = e.target.result;
        }

        reader.readAsDataURL(this.file1);

      }else{
        console.log('현재 파일 선택되지 않음');
      }
    }

  },
  mounted() {
    if(this.file1){
      const reader = new FileReader();
      reader.onload = (e) => {
        this.uploadImageFile = e.target.result;
      }
      reader.readAsDataURL(this.file1);
    }
  }
}
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Roboto:300,900");

.main_con{
  background-color: #3B3B3B;
}
.thumbnail_img{
  background-color: #FFFFFF !important;
  height: 300px;
  width: 300px;
}
.info_table{
  color : #474554;
  border:0;
  letter-spacing: -1px;
}
.label_con{
  border-radius: 15px;
  border:3px solid #FAF8FF;
  background-color: #FFFFFF;
  /*color: #474554;*/
}
.tag_title{
  width: 50px;
  margin:0;
  font-weight: 1000;
  font-size: 24px;
}
.tag_detail{
  width: 250px;
  margin:0;
  font-size: 24px;
}


html,
body {
  /*background: #252833;*/
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
html *,
body * {
  box-sizing: border-box;
}

.cards {
  width: calc(100% - 2em);
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  grid-gap: 1em;
  grid-template-areas: "a a b c" "a a d d";
  width: 80%;
}

.card {
  width: 100%;
  position: relative;
  transition: all 0.25s ease;
  cursor: pointer;
  font-family: "Roboto", sans-serif;
  font-weight: 300;
}
.card:last-child {
  margin-bottom: 0;
}
.card:before {
  height: 0;
  content: "";
  display: block;
  padding-bottom: 47.36%;
}
.card.content:after {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 50%;
  content: "";
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0), black);
}
.card:nth-child(1) {
  grid-area: a;
}
.card:nth-child(2) {
  grid-area: b;
}
.card:nth-child(3) {
  grid-area: c;
}
.card:nth-child(4) {
  grid-area: d;
}
.card-content {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.card-img {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
.card-img img {
  width: 100%;
  height: 100%;
  -o-object-fit: cover;
  object-fit: cover;
}
.card-label {
  position: absolute;
  top: 0.45rem;
  left: 0.45rem;
  background: #089f8a;
  text-transform: uppercase;
  font-weight: 300;
  font-size: 0.7em;
  color: white;
  padding: 0.5em;
}
.card-title {
  position: absolute;
  left: 1em;
  bottom: 1em;
  color: #d6dbeb;
  z-index: 5;
  font-size: 0.8em;
}
.card.form {
  position: relative;
}
.card.form:before {
  background: linear-gradient(60deg, #f79533, #f37055, #ef4e7b, #a166ab, #5073b8, #1098ad, #07b39b, #6fba82);
}
.card.form:after {
  position: absolute;
  top: 0.5em;
  left: 0.5em;
  width: calc(100% - 1em);
  height: calc(100% - 1em);
  content: "";
  background: #fff;
}
.card.form .form-title {
  position: absolute;
  top: 1rem;
  left: 1rem;
  font-size: 2vw;
  font-weight: 900;
  z-index: 5;
  text-transform: uppercase;
  background: linear-gradient(60deg, #f79533, #f37055, #ef4e7b, #a166ab, #5073b8, #1098ad, #07b39b, #6fba82);
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;
}
.card.form .form-title:before {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 100%;
  height: 100%;
  content: "";
  opacity: 0.5;
  filter: blur(10px);
  transition: all 0.25s ease;
  z-index: 2;
  background: linear-gradient(60deg, #f79533, #f37055, #ef4e7b, #a166ab, #5073b8, #1098ad, #07b39b, #6fba82);
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;
  transform: translateX(-50%) translateY(-50%);
}
.card:nth-child(2) .card-label {
  background: #ef4e7b;
}
.card:nth-child(3) .card-label {
  background: #1098ad;
}

</style>
