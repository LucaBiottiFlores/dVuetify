<template>
  <div class="mb-16">

    <v-app-bar app >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <h3>Rick And Morty App</h3>
    </v-app-bar>

    <v-navigation-drawer  absolute app v-model="drawer">
      <v-list-item>
        <v-list-item-content>
          <v-list-item-title>Inicio</v-list-item-title>
          <v-list-item-title>Buscar</v-list-item-title>
          <v-list-item-title>Acerca De</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
     data: () => ({
     drawer: false,
  }),
  name: 'Navbar',
  links: ['Home', 'About Us', 'Team', 'Services', 'Blog', 'Contact Us']
}
</script>

<style></style>
