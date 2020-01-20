<template>
  <Page title="Documentation" icon="mdi-book">
    <h2>
      <nuxt-link to="/doc/setup">Setup son environnement de developpement</nuxt-link>
    </h2>
    <h3>
      Reference Arduino: <a href="https://www.arduino.cc/reference/en/" target="_blank"> https://www.arduino.cc/reference/en/</a>
    </h3>
    <h3>
      Reference lib Adafruit_GFX: <a href="https://cdn-learn.adafruit.com/downloads/pdf/adafruit-gfx.pdf" target="_blank"> https://cdn-learn.adafruit.com/downloads/pdf/adafruit-gfx.pdf</a>
    </h3>
    <h3>
      Documentation lib Fastled: <a href="https://github.com/FastLED/FastLED/wiki/Overview" target="_blank"> https://github.com/FastLED/FastLED/wiki/Overview</a>
    </h3>
     <h3>
      Documentation lib ESPAsyncWebServer: <a href="https://github.com/me-no-dev/ESPAsyncWebServer" target="_blank"> https://github.com/me-no-dev/ESPAsyncWebServer</a>
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
