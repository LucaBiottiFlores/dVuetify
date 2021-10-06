<template>
  <v-app>

    <Navbar />
    <Cards />
    
  </v-app>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Cards from './components/Cards.vue'
export default {
  name: 'App',
  components: { Navbar, Cards },
  data: () => ({
   
  })
}
</script>
