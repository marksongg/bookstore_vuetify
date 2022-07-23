<template>
  <v-card>
    <v-toolbar
          color="success"
          theme="dark"
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Color组件</v-toolbar-title>

      <v-spacer></v-spacer>
    </v-toolbar>
    <div id="box">
      <div class="d-flex just-space-around">
        <v-color-picker v-model="picker" elevation="15"></v-color-picker>
      </div>
    </div>
  </v-card>
</template>

<script>
export default {
  name: 'ColorPickerComp',
  data:()=> ({
    picker: null
  })
}
</script>

<style scoped>
  #box {
    margin: 20px 20px 20px 40px;
  }
</style>