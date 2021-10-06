<template>
  <v-container class="grey background lighten-5">
    <v-row no-glutters>
      <v-col v-for="(personaje, index) in $store.state.personajes"
            :key="index" cols="12" sm="4">
        <v-card class="cardColor mx-auto mt-5 " max-width="400">
          <v-img
          
            class="white--text align-end"
            height="350px"
            :src="personaje.imagen"
          >
            <v-card-title></v-card-title>
          </v-img>
          <v-card-subtitle class="pb-0 "></v-card-subtitle>
          <v-card-text class="text--primary">
            <div>{{ personaje.nombre }}</div>
          </v-card-text>

          <v-card-actions>
         
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'Cards'
}
</script>

<style>
  .cardColor {
background: rgba( 126, 211, 33, 0.25 );
box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
backdrop-filter: blur( 6.5px );
-webkit-backdrop-filter: blur( 6.5px );
border-radius: 10px;
border: 1px solid rgba( 255, 255, 255, 0.18 );
  }
</style>
