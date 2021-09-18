<template>
  <div id="contLogin">
    
    <v-card elevation="15">
        <h2>Login</h2>

      <v-card-text class="text--primary">
        <v-form>
          <v-text-field
            label="Usuario"
            placeholder="Usuario"
            outlined
          ></v-text-field>
          <v-text-field
            label="Contraseña"
            placeholder="Contraseña"
            outlined
          ></v-text-field>
        </v-form>
      </v-card-text>

      <v-card-actions>
        <v-btn color="grey" text> Registrarse </v-btn>

        <v-btn color="orange" text @click="login"> Iniciar Sesión </v-btn>
      </v-card-actions>
    </v-card>
  </div>
</template>

<script>
export default {
    data: ()=>{
        return{

        }
    },
    methods: {
        login(){
            console.log("Verificando credenciales...");
            this.$router.push('/home');
        }
    }
};
</script>

<style lang="scss">
#contLogin {
  width: 400px;
  margin-left: 35%;
  margin-top: 30vh;
  h2{
      text-align: center;
  }
}
</style>
