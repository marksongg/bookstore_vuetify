<template>
  <div id="body1">
    <div class="bg-teal d-flex w-100 align-center px-4" id="foot1">
      <strong class="text-white">请使用电子邮件marksongg@163.com与我联系！</strong>

      <v-spacer></v-spacer>

      <v-btn
        v-for="icon in icons"
        :key="icon"
        class="mx-4 text-white"
        :icon="icon"
        variant="plain"
        size="small"
      ></v-btn>
    </div>

    <div class="px-4 py-2 bg-black text-white text-center w-100">
      {{ new Date().getFullYear() }} - <strong>Vue 3.0 & Vuetify</strong>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BottomComp',
  data(){
    return {
        username: 'Mark',
        icons: [
          'mdi-facebook',
          'mdi-twitter',
          'mdi-linkedin',
          'mdi-instagram',
        ],
        
    }
  }
}
</script>

<style scoped>
  * {
    margin: 0px;
    padding: 0px;
  }

  #body1 {
    margin: 0px;
    padding: 0px;
    font-family: 微软雅黑;
    font-size: 12px;
    width: 100%;
    position: relative;
    left: -256px;
  }

  #foot1 {
    width: 2000px;
  }

 

</style>