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
              <v-col cols="4">
                <v-sheet class="pa-2 ma-2">
                  <ButtonComp2/>
                </v-sheet>
              </v-col>
              <v-col cols="4">
                <v-sheet class="pa-2 ma-2">
                  <ButtonComp3/>
                </v-sheet>
              </v-col>
            </v-row>

            <v-row>
              <v-col cols="4">
                <v-sheet class="pa-2 ma-2">
                  <BreadcrumbsComp/>
                </v-sheet>
              </v-col>
              <v-col cols="4">
                <v-sheet class="pa-2 ma-2">
                  <AlertsComp/>
                </v-sheet>
              </v-col>
              <v-col cols="4">
                <v-sheet class="pa-2 ma-2">
                  <Alerts2Comp/>
                </v-sheet>
              </v-col>
            </v-row>

            <v-row>
                <v-col cols="10">
                  <v-sheet class="pa-2 ma-2">
                    <Alerts3Comp/>
                  </v-sheet>
                </v-col>
            </v-row>

            <v-row>
              <v-col cols="4">
                <v-sheet class="pa-2 ma-2">
                  <ChipsComp2/>
                </v-sheet>
              </v-col>
              <v-col cols="8">
                <v-sheet class="pa-2 ma-2">
                  <DividersComp/>
                </v-sheet>
              </v-col>
            </v-row>

            <v-row>
              <v-col cols="8">
                <v-sheet class="pa-2 ma-2">
                  <ExpansionPanelsComp/>
                </v-sheet>
              </v-col>
            </v-row>

            <v-row>
              <v-col cols="12">
                <v-sheet class="pa-2 ma-2">
                  <CarouselsComp/>
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
import ButtonComp2 from '@/components/ButtonComp2.vue';
import ButtonComp3 from '@/components/ButtonComp3.vue';
import TimelineComp from '@/components/TimelineComp.vue';
import TimelineComp2 from '@/components/TimelineComp2.vue';
import AlertsComp  from '@/components/AlertsComp.vue';
import Alerts2Comp from '@/components/Alerts2Comp.vue';
import Alerts3Comp from '@/components/Alerts3Comp.vue';
import BreadcrumbsComp from '@/components/BreadcrumbsComp.vue';
import ChipsComp2 from '@/components/ChipsComp2.vue';
import DividersComp from '@/components/DividersComp.vue';
import ExpansionPanelsComp from '@/components/ExpansionPanelsComp.vue';
import CarouselsComp from '@/components/CarouselsComp.vue'

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
    ButtonComp2,
    ButtonComp3,
    TimelineComp,
    TimelineComp2,
    AlertsComp,
    Alerts2Comp,
    Alerts3Comp,
    BreadcrumbsComp,
    ChipsComp2,
    DividersComp,
    ExpansionPanelsComp,
    CarouselsComp,
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