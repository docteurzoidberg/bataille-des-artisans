<template>
  <v-app light>
    <Menu />
    <v-content>
      <v-container>
        <div class="logo-container text-center">
          <logo />
        </div>
        <nuxt />
      </v-container>
    </v-content>
    <v-footer
      :fixed="false"
      app
    >
      <span>&copy; 2019</span>
    </v-footer>
  </v-app>
</template>

<script>
import Menu from '~/components/Menu.vue'
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Menu, Logo
  }
}
</script>

<style lang='sass'>
.theme--light.v-application
  background-color: $mytheme-color-teal
.theme--light.v-navigation-drawer
  background-color: $mytheme-color-brownish
  color: $mytheme-color-teal
.theme--dark.v-navigation-drawer
 background-color: $mytheme-color-brownish

h1
  color: $mytheme-color-brownish

</style>
