<template>
  <div class="Lander">
    <v-row align="center" justify="center">
      <v-col cols="12">
        <div class="Lander-imageContainer">
          <v-img
            class="Lander-image"
            max-height="300px"
            max-width="675px"
            src="/this-is-home.png"
          />
          <p class="Lander-text">CONNECT. GROW. SERVE.</p>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import anime from 'animejs/lib/anime.es.js'

export default {
  name: 'HeroComponent',
  mounted() {
    anime
      .timeline({
        targets: '.Lander-text',
        translateY: 300,
        direction: 'reverse',
        easing: 'linear',
        duration: 1000,
      })
      .add({ targets: '.Lander-text', color: 'rgba(255,255,255, .2)' }, 0)
  },
}
</script>

<style lang="scss" scoped>
.Lander {
  margin-top: 300px;
  .Lander-imageContainer {
    width: 100%;
  }
  .Lander-image {
    margin-left: auto;
    margin-right: auto;
  }
  .Lander-text {
    margin-left: auto;
    margin-right: auto;
    margin-top: 35px;
    font-style: italic;
    text-align: center;
    font-size: 36px;
  }
}
</style>
