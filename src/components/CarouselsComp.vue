<template>
  <v-carousel v-model="model">
    <v-carousel-item
      v-for="(color, i) in colors"
      :key="color"
    >
      <v-sheet
        :color="color"
        height="100%"
        tile
      >
        <div class="d-flex fill-height justify-center align-center">
          <div class="text-h2">
            Slide {{ i + 1 }}
          </div>
        </div>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
    name: 'CarouselsComp',
    data: () => ({
        model: 0,
        colors: [
            'primary',
            'secondary',
            'yellow dark-2',
            'red',
            'orange'
        ],
    })
}
</script>

<style>
  .box {
    float: left;
    margin: 10px 0px 10px 10px;
  }
</style>