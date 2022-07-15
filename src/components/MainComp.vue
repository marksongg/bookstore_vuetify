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
        <ImagesComp/>
        <WeatherComp/>
        <MusicComp/>
        <TableComp/>
        <SettingComp/>
        <BannersComp/>
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
import ImagesComp from '@/components/ImagesComp.vue'
import WeatherComp from '@/components/WeatherComp.vue'
import MusicComp from '@/components/MusicComp.vue'
import TableComp from '@/components/TableComp.vue'
import SettingComp from '@/components/SettingComp.vue'
import BannersComp from '@/components/BannersComp.vue'

export default {
  name: 'CenterComp',
  components:{
    TopComp,
    BottomComp,
    ImagesComp,
    WeatherComp,
    MusicComp,
    TableComp,
    SettingComp,
    BannersComp,
  }
  
}
</script>

<style scoped>
  * {
    margin: 0px;
    padding: 0px;
  }

  

</style>