<template>
  <div class="logo-container">
    <v-layout>
      <v-flex valign="center" class="d-flex justify-center align-center fondetoile">
        <img id="logo" src="/logo.svg" width="400" height="250">
      </v-flex>
    </v-layout>
  </div>
</template>

<style lang='sass'>

.logo-container
  margin-top: 10px

#logo
  animation: loading-logo .5s ease-in
  transform-origin: center
  position: absolute
  z-index: 1

.fondetoile
  animation: loading-fond .5s ease-in
  background: url(/fondetoile.svg)
  background-repeat: no-repeat
  background-position: 0 25px
  background-size: 100% 100%
  height: 450px
  width: 100%
  margin-bottom: -50px
  opacity: 1

@keyframes loading-logo
  0%
    transform: scale(0)
  100%
    transform: scale(1)

@keyframes loading-fond
  0%
    opacity: 0
  100%
    opacity: 1
</style>
