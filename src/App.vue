<template>
  <v-app>
    <v-main>
      <CenterComp/>
      <MainComp/>
      <!-- <HelloWorld/> -->
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import CenterComp from './components/CenterComp.vue'
import MainComp from './components/MainComp.vue'

export default {
  name: 'App',

  components: {
    // HelloWorld,
    CenterComp,
    MainComp
  },

  data: () => ({
    //
  }),
}
</script>
