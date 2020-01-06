<template>
  <div class="">
    <img id="logo" src="~/assets/logo.svg">
  </div>
</template>

<style lang='sass'>

#logo
  animation: loading-logo 3s ease-in .1s
  transform-origin: center

@keyframes loading-logo
  0%
    transform: scale(0)
  100%
    transform: scale(1)
</style>
