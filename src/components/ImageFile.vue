<template>
  <div class="content">
    <b-form-file
        v-model="file1"
        :state="Boolean(file1)"
        placeholder="Choose a file or drop it here..."
        drop-placeholder="Drop file here..."
    ></b-form-file>
    <b-button @click="viewFile">파일 확인</b-button>
    <img class="popupImageItem" :src="uploadImageFile" alt="이미지업로드" style="width: 300px; height: 300px;">

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
      console.dir(this.file1)
      const reader = new FileReader();
      reader.onload = (e) => {
        this.uploadImageFile = e.target.result;
      }
      reader.readAsDataURL(this.file1);
    }

  },
  mounted() {
    console.log(this.file1)
  }
}
</script>

<style scoped>

</style>
