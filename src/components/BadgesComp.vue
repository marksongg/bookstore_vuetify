<template>
  <v-row no-gutters>
    <v-btn class="ma-2" variant="text" color="blue-lighten-2">
        <v-badge floating :content="success" color="success" @click="success++">
            <v-icon>mdi-thumb-up</v-icon>
        </v-badge>
    </v-btn>
    <v-btn class="ma-2" variant="text" color="red-lighten-2">
        <v-badge floating :content="error" color="error" @click="error++">
            <v-icon>mdi-thumb-down</v-icon>
        </v-badge>
    </v-btn>
</v-row>
</template>

<script>
export default {
  name: 'BadgesComp',
  data: () => ({
    success: 9,
    error: 2,
  })
}
</script>

<style>

</style>