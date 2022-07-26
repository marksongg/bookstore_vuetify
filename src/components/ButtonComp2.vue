<template>
  <v-card class="card">
    <v-toolbar
          color="secondary"
          theme="dark">
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
        <v-toolbar-title>Button2组件</v-toolbar-title>
        <v-spacer></v-spacer>
    </v-toolbar>
    <div id="buttonDiv">
      <div class="d-flex justify-space-around align-center flex-column flex-md-row fill-height">
        <v-btn
          size="x-small"
          color="secondary"
          >
            Extra small Button
          </v-btn>

          <v-btn
            size="small"
            color="primary"
          >
            Small Button
          </v-btn>
      </div>
      <br/>
      <div class="d-flex justify-space-around align-center flex-column flex-md-row fill-height">
          <v-btn
            color="warning"
          >
            Normal Button
          </v-btn>

          <v-btn
            color="error"
            size="large"
          >
            Large Button
          </v-btn>
        </div>
        <br/>
        <div class="d-flex justify-space-around align-center flex-column flex-md-row fill-height">

          <v-btn
            size="x-large"
            color="success"
          >
            Extra large Button
          </v-btn>
        </div>
        <br/>
        <div class="d-flex justify-space-around align-center flex-column flex-md-row">
          <v-btn
            color="secondary"
            icon="mdi-television"
            size="x-small"
          ></v-btn>

          <v-btn
            color="primary"
            icon="mdi-pencil"
            size="small"
          ></v-btn>
        </div>
        <br/>
        <div class="d-flex justify-space-around align-center flex-column flex-md-row">

          <v-btn
            color="warning"
            icon="mdi-account-circle"
          ></v-btn>

          <v-btn
            color="error"
            icon="mdi-alarm"
            size="large"
          ></v-btn>
          
          <v-btn
            color="success"
            icon="mdi-domain"
            size="x-large"
          ></v-btn>
        </div>
      </div>
  </v-card>
</template>

<script>
export default {
    name: 'ButtonComp2',
    data: () => ({

    })
}
</script>

<style>

  #buttonDiv {
    margin: 10px 10px 10px 10px;
  }
</style>