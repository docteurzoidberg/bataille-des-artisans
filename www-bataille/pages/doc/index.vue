<template>
  <Page title="Documentation" icon="mdi-book">
    <h2>
      <nuxt-link to="/doc/setup">Setup son environnement de developpement</nuxt-link>
    </h2>
    <h3>
      Reference Arduino: <a href="https://www.arduino.cc/reference/en/"> https://www.arduino.cc/reference/en/</a>
    </h3>
    <h3>
      Reference lib Adafruit_GFX: <a href="https://cdn-learn.adafruit.com/downloads/pdf/adafruit-gfx.pdf"> https://cdn-learn.adafruit.com/downloads/pdf/adafruit-gfx.pdf</a>
    </h3>
    <h3>
      Documentation lib Fastled: <a href="https://github.com/FastLED/FastLED/wiki/Overview"> https://github.com/FastLED/FastLED/wiki/Overview</a>
    </h3>
  </Page>
</template>

<script>
import Page from '~/components/Page.vue'
export default {
  components: {
    Page
  }
}
</script>
