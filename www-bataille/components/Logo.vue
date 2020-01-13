<template>
  <div class="logo-container">
    <v-layout>
      <v-flex valign="center" class="d-flex justify-center align-center fondetoile">
        <img id="logo" class="bounce" src="/logo.svg" width="400" height="250">
      </v-flex>
    </v-layout>
  </div>
</template>

<style lang='sass'>

.logo-container
  margin-top: 10px

.fondetoile
  animation: loading-fond 6s ease
  background: url(/fondetoile.svg)
  background-repeat: no-repeat
  background-position: 0 25px
  background-size: 100% 100%
  height: 450px
  width: 100%
  margin-bottom: -50px
  opacity: .9

.bounce
  animation-name: bounce
  -webkit-animation-name: bounce
  animation-duration: 1.6s
  -webkit-animation-duration: 1.6s
  animation-timing-function: ease
  -webkit-animation-timing-function: ease
  transform-origin: 50% 100%
  -ms-transform-origin: 50% 100%
  -webkit-transform-origin: 50% 100%

@keyframes bounce
  0%
    transform: translateY(0%) scaleY(0.6)
  60%
    transform: translateY(-100%) scaleY(1.1)
  70%
    transform: translateY(0%) scaleY(0.95) scaleX(1.05)
  80%
    transform: translateY(0%) scaleY(1.05) scaleX(1)
  90%
    transform: translateY(0%) scaleY(0.95) scaleX(1)
  100%
    transform: translateY(0%) scaleY(1) scaleX(1)

@-webkit-keyframes bounce
  0%
    -webkit-transform: translateY(0%) scaleY(0.6)
  60%
    -webkit-transform: translateY(-100%) scaleY(1.1)
  70%
    -webkit-transform: translateY(0%) scaleY(0.95) scaleX(1.05)
  80%
    -webkit-transform: translateY(0%) scaleY(1.05) scaleX(1)
  90%
    -webkit-transform: translateY(0%) scaleY(0.95) scaleX(1)
  100%
    -webkit-transform: translateY(0%) scaleY(1) scaleX(1)

@keyframes loading-fond
  20%
    opacity: .9
  21%
    opacity: 1
  30%
    opacity: .9
  31%
    opacity: 1
  40%
    opacity: .9

</style>
