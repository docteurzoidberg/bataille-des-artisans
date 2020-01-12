<template>
  <span>
    <v-btn
      v-for="item in items"
      :key="item.title"
      :to="item.to"
      depressed
      large
      icons-and-text
      tile
      color="secondary"
    >
      <v-icon left dark>
        {{ item.icon }}
      </v-icon>
      {{ item.title }}
    </v-btn>
  </span>
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
          icon: 'mdi-gift',
          title: 'Unboxing',
          to: '/unboxing'
        },
        {
          icon: 'mdi-book',
          title: 'Documentation',
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

</style>
