<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm12
      md12
    >
      <v-card>
        <v-card-title class="headline accent--text">
          Bienvenue a la bataille des artisans !
        </v-card-title>
        <v-card-text>
          <p>blabla lorem ipsum papatum</p>
          <p>
            Si vous avez des questions. posez les sur le channel <a
              href="https://factorio.tppt.eu/"
              target="_blank"
              title="discord"
            >
              discord
            </a>.
          </p>
        </v-card-text>
        <v-card-actions>
          <v-spacer />
          <v-btn
            color="primary"
            nuxt
            to="/inspire"
          >
            Continue
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>

</script>

<style>
.logo-container {
  margin-bottom: 10px;
}
</style>
