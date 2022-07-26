<template>
  <v-card>
    <v-toolbar
          color="warning"
          theme="dark"
    >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
        <v-toolbar-title>Alert2组件</v-toolbar-title>
        <v-spacer></v-spacer>
    </v-toolbar>
    <div class="box">
        <p>The v-alert component has multiple customization options such as reducing overall height using or adding a customized border. The following example uses density to reduce the vertical space needed for the component:</p>
        <v-alert
      density="compact"
      type="info"
    >
      I'm a compact alert with a <strong>type</strong> of info
    </v-alert>

    <br>

    <v-alert
      density="comfortable"
      type="success"
      variant="tonal"
    >
      I'm a comfortable alert with the <strong>text</strong> prop and a <strong>type</strong> of success
    </v-alert>

    <br>

    <v-alert
      border="start"
      density="default"
      type="warning"
    >
      I'm a default alert with the <strong>border</strong> prop and a <strong>type</strong> of warning
    </v-alert>

    <br>

    <!-- Density is "default" by default -->
    <v-alert
      prominent
      type="error"
      variant="outlined"
    >
      I'm a default alert with the <strong>prominent</strong> prop and a <strong>type</strong> of error
    </v-alert>
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