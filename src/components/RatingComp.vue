<template>
  <div class="text-center">
    <v-rating
      v-model="rating"
      clearable
    ></v-rating>
  </div>
</template>

<script>
export default {
  name: 'RatingComp',
  data: ()=> ({
    rating: 3,
  })
}
</script>

<style scoped>

</style>