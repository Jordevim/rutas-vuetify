<template>
  <div>
      <h1>EMPRENDETE</h1>
      
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
