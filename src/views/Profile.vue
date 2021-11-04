<template>
  <div >
    <b-container class="bg-info main_con ">
      <b-row>
        <b-col v-for="i in 12" :key="i+`_1`" class="p-2">A</b-col>
      </b-row>
      <b-row class="h-50">
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
}

</style>
