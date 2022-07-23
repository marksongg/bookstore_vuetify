<template>
  <v-card>
    <v-toolbar
          color="info"
          theme="dark"
    >
      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>Timeline组件</v-toolbar-title>

      <v-spacer></v-spacer>
    </v-toolbar>
    <v-timeline direction="horizontal">
      <v-timeline-item>
        <template v-slot:opposite>
          Opposite content
        </template>
        <div>
          <div class="text-h6">Content title</div>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          Opposite content
        </template>
        <div>
          <div class="text-h6">Content title</div>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          </p>
        </div>
      </v-timeline-item>

      <v-timeline-item>
        <template v-slot:opposite>
          Opposite content
        </template>
        <div>
          <div class="text-h6">Content title</div>
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          </p>
        </div>
      </v-timeline-item>
    </v-timeline>
  </v-card>
</template>

<script>
  export default {
    name: 'TimelineComp'
  }
</script>

<style scoped>

</style>