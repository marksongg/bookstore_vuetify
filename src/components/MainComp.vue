<template>
  <div>
    <v-navigation-drawer app>
      <!-- -->
      <TopComp/>
    </v-navigation-drawer>
    
    <!-- Sizes your content based upon application components -->
    <v-main>
      
      <!-- Provides the application the proper gutter -->
      <v-container fluid>
      
        <!-- If using vue-router -->
        <router-view></router-view>
      </v-container>
    </v-main>

    <v-footer app>
      <!-- -->
      <BottomComp/>
    </v-footer>
  </div>
</template>

<script>
import TopComp from '@/components/TopComp.vue'
import BottomComp from '@/components/BottomComp.vue'

export default {
  name: 'CenterComp',
  components:{
    TopComp,
    BottomComp
  }
  
}
</script>

<style scoped>
  * {
    margin: 0px;
    padding: 0px;
  }

  

</style>