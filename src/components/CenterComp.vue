<template>
  <div>
    <v-toolbar dark prominent src="@/assets/vbanner.jpg">
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>首页</v-toolbar-title>
      <v-toolbar-title>新书</v-toolbar-title>
      <v-toolbar-title>特价书</v-toolbar-title>
      <v-toolbar-title>教材</v-toolbar-title>
      <v-toolbar-title>畅销榜</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn icon>
        <v-icon>mdi-export</v-icon>
      </v-btn>
    </v-toolbar>
  </div>
</template>

<script>
export default {
  name: 'CenterComp',
}
</script>

<style scoped>
  * {
    margin: 0px;
    padding: 0px;
  }

  #body1 {
    background-color: #030303;
    width: 100%;
    margin: 0px auto;
    font-family: 微软雅黑;
    font-size: 48px;
    height: 120px;
  }

  #box {
    height: 200px;
  }

  #logo {
    border: solid 2px #FFF;
    float: left;
    margin-top: 20px;
    margin-left: 10px;
  }

  #user {
    float: right;
    margin-top: 20px;
    margin-right: 20px;
  }

  #avatar {
    color: #F3F3F3;
  }

</style>