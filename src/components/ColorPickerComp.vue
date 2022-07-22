<template>
  <div class="d-flex just-space-around">
    <v-color-picker v-model="picker" elevation="15"></v-color-picker>
  </div>
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

</style>