<template>
  <div>
    <v-navigation-drawer app>
      <!-- -->
      <TopComp/>
    </v-navigation-drawer>
    
    <!-- Sizes your content based upon application components -->
    <v-main>
      
      <!-- Provides the application the proper gutter -->
      <div id="gridLayout">
        <v-container fluid>
          <!-- <v-container class="bg-surface-variant"> --> 
          <v-container>
            <v-row no-gutters>
              <v-col>
                <v-sheet class="pa-2 ma-2">
                  <!-- .v-col-auto -->
                  <ChipsComp/>
                </v-sheet>
              </v-col>
              <v-col>
                <v-sheet class="pa-2 ma-2">
                  <!-- .v-col-auto -->
                  <BannersComp/>
                </v-sheet>
              </v-col>
              <v-col>
                <v-sheet class="pa-2 ma-2">
                  <!-- .v-col-auto -->
                  <TableComp/>
                </v-sheet>
              </v-col>
            </v-row>

            <v-row no-gutters>
              <v-col>
                <v-sheet class="pa-2 ma-2">
                  <!-- .v-col-auto -->
                  <SettingComp/>
                </v-sheet>
              </v-col>
              <v-col>
                <v-sheet class="pa-2 ma-2">
                  <!-- .v-col-auto -->
                  <ImagesComp/>
                </v-sheet>
              </v-col>
              <v-col>
                <v-sheet class="pa-2 ma-2">
                  <!-- .v-col-auto -->
                  <MusicComp/>
                </v-sheet>
              </v-col>
            </v-row>

            <v-row no-gutters>
              <v-col cols="4">  <!-- ★占用2列  -->
                <v-sheet class="pa-2 ma-2">
                  <WeatherComp/>
                </v-sheet>
              </v-col>
              <v-col>
                <v-sheet class="pa-2 ma-2">
                  <!-- .v-col-auto -->
                  <ColorPickerComp/>
                </v-sheet>
              </v-col>
              <v-col>
                <v-sheet class="pa-2 ma-2">
                  <!-- .v-col-auto -->
                  <TransitionComp/>
                </v-sheet>
              </v-col>
            </v-row>

            <v-row no-gutters>
              <v-col cols="12">
                <v-sheet class="pa-2 ma-2">
                  <!-- .v-col-auto -->
                  <TimelineComp/>
                </v-sheet>
              </v-col>
            </v-row>

            <v-row no-gutters>
              <v-col cols="4">
                <v-sheet class="pa-2 ma-2">
                  <TimelineComp2/>
                </v-sheet>
              </v-col>

              <v-col>
                <v-sheet class="pa-2 ma-2">
                  <FormInputComp/>
                </v-sheet>
              </v-col>
            </v-row>

            <v-row>
              <v-col cols="4">
                <v-sheet class="pa-2 ma-2">
                  <ButtonComp/>
                </v-sheet>
              </v-col>
            </v-row>
          </v-container>

          
          
          <!-- If using vue-router -->
          <router-view></router-view>
        </v-container>
      </div>
    </v-main>

    <v-footer app>
      <!-- -->
      <BottomComp/>
    </v-footer>
  </div>
</template>

<script>
import TopComp from '@/components/TopComp.vue';
import BottomComp from '@/components/BottomComp.vue';
import ImagesComp from '@/components/ImagesComp.vue';
import WeatherComp from '@/components/WeatherComp.vue';
import MusicComp from '@/components/MusicComp.vue';
import TableComp from '@/components/TableComp.vue';
import SettingComp from '@/components/SettingComp.vue';
import BannersComp from '@/components/BannersComp.vue';
import ChipsComp from '@/components/ChipsComp.vue';
import FormInputComp from '@/components/FormInputComp.vue';
import ColorPickerComp from '@/components/ColorPickerComp.vue';
import TransitionComp from '@/components/TransitionComp.vue';
import ButtonComp from '@/components/ButtonComp.vue';
import TimelineComp from '@/components/TimelineComp.vue';
import TimelineComp2 from '@/components/TimelineComp2.vue';

export default {
  name: 'MainComp',
  components:{
    TopComp,
    BottomComp,
    ImagesComp,
    WeatherComp,
    MusicComp,
    TableComp,
    SettingComp,
    BannersComp,
    ChipsComp,
    FormInputComp,
    ColorPickerComp,
    TransitionComp,
    ButtonComp,
    TimelineComp,
    TimelineComp2
  }
  
}
</script>

<style scoped>
  * {
    padding: 0px;
  }

  #gridLayout {
    margin-top: 10px;
    margin-left: -300px;
    margin-right: 0px;
  }

  

</style>