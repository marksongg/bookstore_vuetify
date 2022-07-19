<template>
  <div id="body1">
     <div class="text-center">
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
      </div>
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
        'vue 3.0', 'Spring boot'
      ],
      devTools: [
        'Eclipse', 'VS code', 'Visual Studio', 'JetBrains'
      ],
      plugInComponents: [
        'Vuetify', 'ActiveReport'
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