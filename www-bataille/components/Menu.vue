<template>
  <v-navigation-drawer
    absolute
    permanent
    right
    app
    dark
  >
    <v-list dense>
      <v-list-item
        v-for="item in items"
        :key="item.title"
        @click=""
        :to="item.to"
      >
        <v-list-item-icon>
          <v-icon>{{ item.icon }}</v-icon>
        </v-list-item-icon>
        <v-list-item-content>
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item-content>
      </v-list-item>
      <v-divider />
    </v-list>
  </v-navigation-drawer>
  </v-card>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          icon: 'mdi-home',
          title: 'Accueil',
          to: '/'
        },
        {
          icon: 'mdi-book',
          title: 'Documentations',
          to: '/doc'
        },
        {
          icon: 'mdi-trophy',
          title: 'Epreuves',
          to: '/epreuves'
        }
      ],
      title: 'La Bataille Des Artisans'
    }
  }
}
</script>

<style lang="sass">
.v-list .v-list-item--active
  color: $mytheme-color-teal
</style>
