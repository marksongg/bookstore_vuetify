<template>
  <v-timeline side="end">
    <v-timeline-item
      v-for="item in items"
      :key="item.id"
      :dot-color="item.color"
      size="small"
    >
      <v-alert
        :value="true"
        :color="item.color"
        :icon="item.icon"
        class="white--text"
      >
        {{item.msg}}
      </v-alert>
    </v-timeline-item>
  </v-timeline>
</template>

<script>
  export default {
    name: 'TimelineComp2',
    data: () => ({
      items: [
        {
          id: 1,
          color: 'info',
          icon: 'mdi-information',
          msg: 'info: Go to School'
        },
        {
          id: 2,
          color: 'error',
          icon: 'mdi-anchor',
          msg: 'error: Do homework'
        },
        {
          id: 3,
          color: 'secondary',
          icon: 'mdi-apple-icloud',
          msg: 'secondary: Do homework'
        },
        {
          id: 4,
          color: 'primary',
          icon: 'mdi-apps-box',
          msg: 'primary: Go to School'
        },
        {
          id: 5,
          color: 'success',
          icon: 'mdi-boomerang',
          msg: 'success: Do homework'
        },
        {
          id: 6,
          color: 'white',
          icon: 'mdi-bridge',
          msg: 'white: Do homework'
        },
        {
          id: 7,
          color: 'warning',
          icon: 'mdi-cog-outline',
          msg: 'warning: Go Climbing'
        }
      ]
    })
  }
</script>

<style scoped>

</style>