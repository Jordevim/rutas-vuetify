<template>
  <div>
      <h1>EMPRENDETE</h1>

      <v-carousel
    cycle
    height="400"
    hide-delimiter-background
    show-arrows-on-hover
  >
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
      <v-sheet
        :color="colors[i]"
        height="100%"
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <div class="text-h2">
            {{ slide }} Slide
          </div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
  </div>
</template>

<script>

import store from '../store/index.js'

export default {
    data: ()=>{
        return{

        }
    },
    methods: {

    },
    created: ()=>{
        store.dispatch('getPersonajes');
    }
}
</script>

<style>

</style>
