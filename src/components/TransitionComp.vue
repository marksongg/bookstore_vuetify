<template>
  <v-hover v-slot="{ isHovering, props }">
    <v-card
      class="mx-auto"
      color="grey-lighten-4"
      max-width="600"
      v-bind="props"
    >
      <v-toolbar
          color="primary"
          theme="dark"
      >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title>Transition组件</v-toolbar-title>

        <v-spacer></v-spacer>
      </v-toolbar>
      <v-img
        :aspect-ratio="16/9"
        cover
        src="https://cdn.vuetifyjs.com/images/cards/kitchen.png"
      >
        <v-expand-transition>
          <div
            v-if="isHovering"
            class="d-flex transition-fast-in-fast-out bg-orange-darken-2 v-card--reveal text-h2 text-white"
            style="height: 100%;"
          >
            $14.99
          </div>
        </v-expand-transition>
      </v-img>
      <v-card-text
        class="pt-6"
        style="position: relative;"
      >
        <div class="font-weight-light text-grey text-h6 mb-2">
          For the perfect meal
        </div>
        <h3 class="text-h4 font-weight-light text-orange mb-2">
          QW cooking utensils
        </h3>
        <div class="font-weight-light text-h6 mb-2">
          Our Vintage kitchen utensils delight any chef.<br>
          Made of bamboo by hand
        </div>
        
        <RatingComp/>
        <BadgesComp/>
      </v-card-text>
    </v-card>
  </v-hover>
  
</template>

<script>
import RatingComp from '@/components/RatingComp.vue';
import BadgesComp from '@/components/BadgesComp.vue';

export default {
    name: 'TransitionComp',
    data: () => ({
        rating: 3,  
    }),
    components:{
        RatingComp,
        BadgesComp
    }
}

</script>

<style scoped>
    .v-card--reveal {
        align-items: center;
        bottom: 0;
        justify-content: center;
        opacity: .9;
        position: absolute;
        width: 100%;
    }
</style>