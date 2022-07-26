<template>
  <div class="box">
    <v-card>
      <v-toolbar
            color="warning"
            theme="dark"
      >
          <v-app-bar-nav-icon></v-app-bar-nav-icon>
          <v-toolbar-title>Alert组件</v-toolbar-title>
          <v-spacer></v-spacer>
      </v-toolbar>
      <div class="alertCard">
        <v-alert
          color="yellow-darken-4"
          icon="mdi-flash"
          title="Flat (Default)"
          variant="flat"
        >
          Nullam tincidunt adipiscing enim. In consectetuer turpis ut velit. Maecenas egestas arcu quis ligula mattis placerat. Praesent metus tellus, elementum eu, semper a, adipiscing nec, purus.
        </v-alert>

        <br>

        <v-alert
          color="info"
          title="Tonal"
          variant="tonal"
        >
          <div>
            Maecenas nec odio et ante tincidunt tempus. Sed mollis, eros et ultrices tempus, mauris ipsum aliquam libero, non adipiscing dolor urna a orci. Proin viverra, ligula sit amet ultrices semper, ligula arcu tristique sapien, a accumsan nisi mauris ac eros. Curabitur turpis.
          </div>

          <v-divider class="my-4 bg-light-blue-lighten-4"></v-divider>

          <div class="d-flex flex-row align-center justify-space-between">
            <div>
              Proin magna. Vivamus in erat ut urna cursus vestibulum. Etiam imperdiet imperdiet orci.
            </div>

            <v-btn
              color="info"
              variant="outlined"
            >
              Okay
            </v-btn>
          </div>
        </v-alert>

        <br>

        <v-alert
          color="deep-orange"
          icon="mdi-fire"
          title="Outlined"
          variant="outlined"
        >
          Nullam tincidunt adipiscing enim. In consectetuer turpis ut velit. Maecenas egestas arcu quis ligula mattis placerat. Praesent metus tellus, elementum eu, semper a, adipiscing nec, purus.
        </v-alert>

        <br>

        <v-alert
          border="start"
          color="teal-darken-4"
          density="compact"
          icon="mdi-clock-fast"
          title="Elevated"
          variant="elevated"
        >
          Vestibulum ullamcorper mauris at ligula. Nulla porta dolor. Vestibulum facilisis, purus nec pulvinar iaculis, ligula mi congue nunc, vitae euismod ligula urna in dolor. Curabitur at lacus ac velit ornare lobortis.
        </v-alert>

        <br>

        <v-alert
          icon="mdi-cloud-alert"
          prominent
          title="Text"
          type="error"
          variant="text"
        >
          Praesent blandit laoreet nibh. Praesent nonummy mi in odio. Phasellus tempus. Mauris turpis nunc, blandit et, volutpat molestie, porta ut, ligula. Duis leo.
        </v-alert>

        <br>

        <v-alert
          color="orange"
          density="compact"
          icon="mdi-note"
          prominent
          title="Plain"
          variant="plain"
        >
          Vestibulum ullamcorper mauris at ligula. Nulla porta dolor. Vestibulum facilisis, purus nec pulvinar iaculis, ligula mi congue nunc, vitae euismod ligula urna in dolor. Curabitur at lacus ac velit ornare lobortis.
        </v-alert>
      </div>
    </v-card>
  </div>
</template>

<script>
export default {
    name: 'Alerts3Comp'
}
</script>

<style scoped>
  .alertCard {
    margin: 10px 10px 10px 10px;
  }

  .box {
    margin-left: 100px;

  }


</style>