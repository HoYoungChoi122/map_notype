<template>
  <div class="home">
    <div v-if="isMap">
      <img alt="Vue logo" src="../assets/logo.png">
      <KakaoMap msg="Welcome to Your Vue.js App"/>
    </div>
    <div v-else>
      <ImageFile/>
    </div>

  </div>
</template>

<script>
// @ is an alias to /src
import KakaoMap from '@/components/KakaoMap.vue'
import ImageFile from '@/components/ImageFile.vue'

export default {
  name: 'Home',
  components: {
    KakaoMap,
    ImageFile
  },
  data: () => ({
    isMap : false
  }),
}
</script>
