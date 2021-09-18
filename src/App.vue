<template>
  <v-app>
    <v-app-bar
      app
      color= #48C9B0
      dark
    >
      <div class="d-flex align-center">
        <h1>EMPRENDETE</h1>        
      
      </div>

      <v-spacer></v-spacer>

      <v-btn
        
        target="_blank"
        text
      >
        <span class="mr-2">Inicio</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>
