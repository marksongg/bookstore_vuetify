<template>
  <v-card>
    <v-toolbar
          color="warning"
          theme="dark"
    >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
        <v-toolbar-title>Alert组件</v-toolbar-title>
        <v-spacer></v-spacer>
    </v-toolbar>
    <div class="box">
        <v-alert type="success">I'm a success alert.</v-alert>
        <br>
        <v-alert type="info">I'm an info alert.</v-alert>
        <br>
        <v-alert type="warning">I'm a warning alert.</v-alert>
        <br>
        <v-alert type="error">I'm an error alert.</v-alert>
    </div>
  </v-card>
</template>

<script>
export default {
    name: 'AlertsComp'
}
</script>

<style scoped>
  .box {
    float: left;
    margin: 10px 0px 10px 10px;
  }
</style>