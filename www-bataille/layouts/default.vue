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
body
  font-family: sans-serif
html
  overflow-y: auto
.v-app-bar
  font-family: 'Jockey One', sans-serif
h1, h2, h3
  font-family: 'Jockey One', sans-serif
  padding-top: 10px
  padding-bottom: 10px

@media (min-width: 1904px)
  .container
    max-width: 1280px !important
.logo-container
  margin-bottom: 10px
h1
  display: block
  padding-bottom: 10px
  width: 100%
  border-bottom: 2px solid $mytheme-color-teal
  color: $mytheme-color-brownish
h2
  margin-bottom: 10px
</style>

</style>
