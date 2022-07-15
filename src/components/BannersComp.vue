<template>
  <div id="body1">
    <div id="box">
       <v-banner
          lines="one"
          icon="mdi-lock"
          color="deep-purple-accent-4"
          class="my-4"
        >
          <v-banner-text>
            Banner with one line of text.
          </v-banner-text>

          <template v-slot:actions>
            <v-btn>Action</v-btn>
          </template>
        </v-banner>

        <v-banner
          lines="two"
          icon="mdi-weather-hurricane"
          color="error"
          class="my-4"
        >
          <v-banner-text>
            Banner with two lines of text. If the text is too long to fit on two lines then an ellipsis will be ...
          </v-banner-text>

          <template v-slot:actions>
            <v-btn>Action</v-btn>
          </template>
        </v-banner>

        <v-banner
          lines="three"
          icon="$warning"
          color="warning"
          class="my-4"
        >
          <v-banner-text>
            Banner with three lines of text. One or two lines is preferable. 
          </v-banner-text>

          <template v-slot:actions>
            <v-btn>Action</v-btn>
          </template>
        </v-banner>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BannersComp',
  data(){
    return {

    }
  }
}
</script>

<style scoped>
  * {
    margin: 0px;
    padding: 0px;
  }

  #box {
    float: right;
  }

</style>