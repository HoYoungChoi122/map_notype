<template>
  <div >
    <b-container class="main_con text-white pl-5 pt-5 text-left">
      <b-row class="pl-2 pr-2">
        <b-col cols="2">
          <b-icon stacked icon="slash-circle" variant="danger" style="width: 100px; height: 100px;"></b-icon>
        </b-col>
        <b-col cols="1"></b-col>
      </b-row>
      <b-row class="h-25 w-50">
        <b-col class="pt-3">
          <h1>TEST PAGE</h1>
          <h1>TEST PAGE</h1>
        </b-col>
      </b-row>
      <b-row class="pl-2 pr-2">
        <b-col v-for="i in 12" :key="i+`_1`">1</b-col>
      </b-row>
    </b-container>
  </div>

</template>

<script>
export default {
  name: "Profile"
}
</script>

<style scoped>
.main_con{
  height: 768px;
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
</style>
