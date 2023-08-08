<template>
<v-app>
  <v-content>
    <v-container class="fill-height" fluid>
      <v-row align="center" justify="center">
       <v-col cols="12" sm="8" md="8">
<v-card class="elevation-12">
  <v-window v-model="step">
    <v-window-item :value="1">
<v-row>
  <v-col cols="12" md="8">
    <v-card-text class="mt-12">
<h2 class="text-center display-2 teal--text text--acent-3">Sign Up</h2>
<div class="text-center" mt-4>
  <v-btn class="mx-2" fab color="black" outlined>
<v-icon>mdi-facebook</v-icon>
  </v-btn>
  <v-btn class="mx-2" fab color="black" outlined>
<v-icon>mdi-email</v-icon>
  </v-btn>
  <v-btn class="mx-2" fab color="black" outlined>
<v-icon>mdi-facebook</v-icon>
  </v-btn>
</div>
<h4 class="text-center mlt-4">Insere ton email pour veriication</h4>
 <v-form>
  <v-text-field 
  label="Email"
  name="Email"
  prepend-icon="mdi-email"
  type="text"
  color="blue darken-3"
  />

  <v-text-field 
  label="Password"
  id="password"
  name="password"
  type="password"
  color="blue darken-3"
  prepend-icon="mdi-lock"
  />

 </v-form>
 <h3 class="text-cener mt-3">Mot de Passe Oublié</h3>
</v-card-text>
<div class="text-center mb-3">
  <v-btn rounded color="blue darken-3 dark">Sign iN</v-btn>
</div>
  </v-col>
  <v-col cols="12" md="4" class="blue darken-3">
    <v-card-text class="white--text mt-12">
      <h1 class="text-center display-1">Hello, Friends</h1>
      <h5 class="text-center ">Entrez vos donnés personnels</h5>
    </v-card-text>

    <div class="text-center">
      <v-btn rounded outlined="" dark @click="step++">SIGN UP</v-btn>
    </div>
  </v-col>
</v-row>
    </v-window-item>
    <v-window-item :value="2">
      <v-row class="fill-height">
  <v-col cols="12" md="4" class="blue darken-3">
<v-card-text class="whie-text mt-12">
  <h1 class="text-center display-1">Welcome back, Friends</h1>
  <h5 class="text-center ">To keep connected with us please login with your personnel info</h5>
</v-card-text>
<div class="text-center">
      <v-btn rounded outlined="" dark @click="step++">SIGN UP</v-btn>
</div>
  </v-col>
  <v-col cols="12" md="8">
    <h1 class="text-center display-2 teal--text text-accent-3">Create Account</h1>
<div class="text-center mt-4">
  <v-btn class="mx-2" fab color="black" outlined>
<v-icon>mdi-facebook</v-icon>
  </v-btn>
  <v-btn class="mx-2" fab color="black" outlined>
<v-icon>mdi-email</v-icon>
  </v-btn>
  <v-btn class="mx-2" fab color="black" outlined>
<v-icon>mdi-facebook</v-icon>
  </v-btn>
</div>
<h4 class="text-center mlt-4">Insere ton email pour veriication</h4>
 <v-form>
  <v-text-field 
  label="Email"
  name="Email"
  prepend-icon="mdi-email"
  type="text"
  color="blue darken-3"
  />

  <v-text-field 
  label="Password"
  id="password"
  name="password"
  type="password"
  color="blue darken-3"
  prepend-icon="mdi-lock"
  />

 </v-form>
 <div class="text-center mb-3">
  <v-btn rounded color="blue darken-3 dark">Sign iN</v-btn>
</div>
  </v-col>
</v-row>
</v-window-item>
  </v-window>
</v-card>
       </v-col> 
      </v-row>
    </v-container>
  </v-content>
</v-app>
</template>
<script>

  export default {
    name: 'HelloWorld',

    data: () => ({
    step:1
    }),
    props:{
      source: String
    }
  };
</script>



