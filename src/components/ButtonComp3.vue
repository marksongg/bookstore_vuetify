<template>
  <v-card class="card">
    <v-toolbar
          color="error"
          theme="dark">
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
        <v-toolbar-title>Button3组件</v-toolbar-title>
        <v-spacer></v-spacer>
    </v-toolbar>
    <div class="box">
      <v-btn
        color="primary"
      >
        Normal Button
      </v-btn>

      <v-btn
        rounded="lg"
        color="primary"
      >
        Rounded Button
      </v-btn>

      <v-btn
        :rounded="0"
        color="primary"
      >
        Tile Button
      </v-btn>

      <v-btn
        rounded="pill"
        color="primary"
      >
        Pill Button
      </v-btn>
    </div>
  </v-card>
</template>

<script>
export default {
    name: 'ButtonComp3',
    data: () => ({

    })
}
</script>

<style>

  .box {
    float: left;
  }

  .box button {
    margin: 10px 10px 10px 10px;
  }
</style>