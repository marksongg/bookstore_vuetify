<template>
  <div id="body1">
      <v-card>
        <v-toolbar
          color="deep-purple accent-4"
          theme="dark"
        >
          <v-app-bar-nav-icon></v-app-bar-nav-icon>

          <v-toolbar-title>自我介绍 (Chips组件)</v-toolbar-title>

          <v-spacer></v-spacer>

          <!-- <v-btn icon>
            <v-icon>mdi-magnify</v-icon>
          </v-btn> -->
        </v-toolbar>
        <v-chip
          class="ma-2"
          color="indigo"
          text-color="white"
          prepend-icon="mdi-account-circle"
        >
          Mark
        </v-chip>

        <v-chip
          class="ma-2"
          color="orange"
          text-color="white"
          append-icon="mdi-star"
        >
          2005年计算机科学与技术本科毕业
        </v-chip>

        <v-chip
          class="ma-2"
          color="primary"
          text-color="white"
          append-icon="mdi-cake-variant"
        >
          {{ new Date().getFullYear() - 2005 }}年软件开发经验
        </v-chip>

        <v-chip
          class="ma-2"
          color="green"
          text-color="white"
          append-icon="mdi-car"
        >
          最近恶补前端技术，持续冲电中。
        </v-chip>

        <v-chip
          class="ma-2"
          color="warning"
          text-color="white"
          append-icon="mdi-cloud"
        >
          汽车贩卖，广告，电力ERP，银行，保险，电信等相关业务经验
        </v-chip>

        <v-chip
          v-for="developLanguage in developLanguages"
          :key="developLanguage"
          class="ma-2"
          color="teal"
          text-color="white"
          prepend-icon="mdi-checkbox-marked-circle"
          :model-value="true"
        >
          {{developLanguage}}
        </v-chip>

        <v-chip
          v-for="db in dbs"
          :key="db"
          class="ma-2"
          color="pink"
          text-color="white"
          prepend-icon="mdi-checkbox-marked-circle"
          :model-value="true"
        >
          {{db}}
        </v-chip>

        <v-chip
          v-for="framework in frameworks"
          :key="framework"
          class="ma-2"
          color="blue"
          text-color="white"
          prepend-icon="mdi-checkbox-marked-circle"
          :model-value="true"
        >
          {{framework}}
        </v-chip>

        <v-chip
          v-for="devTool in devTools"
          :key="devTool"
          class="ma-2"
          color="orange"
          text-color="white"
          prepend-icon="mdi-checkbox-marked-circle"
          :model-value="true"
        >
          {{devTool}}
        </v-chip>

        <v-chip
          v-for="plugInComponent in plugInComponents"
          :key="plugInComponent"
          class="ma-2"
          color="grape"
          text-color="white"
          prepend-icon="mdi-checkbox-marked-circle"
          :model-value="true"
        >
          {{plugInComponent}}
        </v-chip>

        <v-chip
          class="ma-2"
          closable
          color="red"
          text-color="white"
          close-icon="mdi-delete"
          prepend-icon="mdi-checkbox-marked-circle"
          :model-value="true"
          @click="close"
        >
          Click me can delete!
        </v-chip>
      </v-card>
  </div>
</template>

<script>
export default {
  name: 'ChipsComp',
  data(){
    return {
      settings: [],
      developLanguages: [
        'JAVA','C#','VB','Delphi'
      ],
      dbs :[
        'Oracle','MS Server', 'MySql','Elastic Search','Cassandora'
      ],
      frameworks: [
        'Vue', 'Angular','Spring boot'
      ],
      devTools: [
        'Eclipse', 'STS', 'VS code', 'Visual Studio', 'JetBrains'
      ],
      plugInComponents: [
        'Vuetify', 'Bootstrap', 'ActiveReport'
      ]
    }
  },
  methods: {
    close () {
      alert('Chip close clicked')
    },
  }
}
</script>

<style scoped>
  * {
    margin: 0px;
    padding: 0px;
  }

</style>