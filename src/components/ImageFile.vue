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
    <img class="popupImageItem"  alt="이미지업로드" style="width: 300px; height: 300px;">
<!--    <b-img thumbnail fluid :src="uploadImageFile" alt="Image 1"></b-img>-->
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
    프로필?

    <b-container fluid class="p-4 bg-info container">
      <b-row>
        <div class="container mt-5 mb-5">
          <div class="row no-gutters">
            <div class="col-md-4 col-lg-4"><b-img thumbnail  :src="uploadImageFile" alt="프로필 사진"/></div>
            <div class="col-md-8 col-lg-8">
              <div class="d-flex flex-column">
                <div class="d-flex flex-row justify-content-between align-items-center p-5 bg-dark text-white">
                  <h3 class="display-5">최호영</h3>
                  <span></span>
                  <span></span>
                  <span>회사 : 피앰아이</span>
                  <span>소속 : 개발부</span>
                  <!--              <span>소속 : 개발부</span>-->
                  <!--              <span>소속 : 개발부</span>-->
                </div>
                <div class="p-3 bg-black text-white">
                  <h6>Web designer &amp; Developer</h6>
                </div>
                <div class="d-flex flex-row text-white">
                  <div class="p-4 bg-primary text-center skill-block">
                    <h4>90%</h4>
                    <h6>Bootstrap</h6>
                  </div>
                  <div class="p-3 bg-success text-center skill-block">
                    <h4>70%</h4>
                    <h6>Jquery</h6>
                  </div>
                  <div class="p-3 bg-warning text-center skill-block">
                    <h4>80%</h4>
                    <h6>HTML</h6>
                  </div>
                  <div class="p-3 bg-danger text-center skill-block">
                    <h4>75%</h4>
                    <h6>PHP</h6>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </b-row>
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
    // console.log(this.file1)
    if(this.file1){
      console.dir(this.file1)
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
img {
  width: 100%;
  height: 100%
}

.bg-black {
  background: #000
}

.skill-block {
  width: 30%
}

@media (min-width: 991px) and (max-width:1200px) {
  .skill-block {
    padding: 32px !important
  }
}

@media (min-width: 1200px) {
  .skill-block {
    padding: 56px !important
  }
}

body {
  background-color: #eeeeee
}
</style>
