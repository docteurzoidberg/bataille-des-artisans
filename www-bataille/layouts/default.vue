<template>
  <v-app>
    <Navbar />
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
import Navbar from '~/components/Navbar.vue'
export default {
  components: {
    Navbar
  }
}
</script>

<style lang='sass'>
.theme--light.v-application
  background-color: $mytheme-color-teal
.theme--light.v-navigation-drawer
  color: $mytheme-color-teal
html
  overflow-y: auto
*
  font-family: 'Jockey One', sans-serif
h1
  color: $mytheme-color-brownish

</style>
