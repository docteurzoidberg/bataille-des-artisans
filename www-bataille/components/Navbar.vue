<template>
  <div>
    <v-app-bar fixed large dark color="secondary">
      <v-toolbar-title>
        <router-link to="/" tag="span" style="cursor: pointer" class=".display-1">
          {{ appTitle }}
        </router-link>
      </v-toolbar-title>
      <v-spacer />
      <Menu />
    </v-app-bar>
    <Logo />
  </div>
</template>

<script>
import Menu from '~/components/Menu.vue'
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Menu, Logo
  },
  data () {
    return {
      appTitle: 'BATAILLE DES ARTISANS'
    }
  }
}
</script>

<style scoped lang='sass'>
  .v-toolbar__title
    font-size: 1.5rem
</style>
