<template>
  <div class="Lander">
    <v-row align="center" justify="center">
      <v-col cols="12">
        <div class="Lander-imageContainer" :style="{ opacity: opacity }">
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
  data() {
    return {
      opacity: 1,
      myScrollY: 0,
    }
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll)
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
  methods: {
    handleScroll(event) {
      let verticalScrollValue = event.path[1].scrollY

      console.log('WINDOWS SCROLLY', verticalScrollValue)
      console.log('TYLER SCROLL Y', this.myScrollY)

      if (verticalScrollValue > 150 && verticalScrollValue > this.myScrollY) {
        if (this.opacity > 0) {
          this.opacity = this.opacity - 0.01
        }
      } else if (
        verticalScrollValue < 600 &&
        verticalScrollValue < this.myScrollY
      ) {
        if (this.opacity < 1) {
          this.opacity = this.opacity + 0.01
        }
      }

      this.myScrollY = verticalScrollValue
    },
  },
}
</script>

<style lang="scss" scoped>
.Lander {
  margin-top: 300px;
  .Lander-imageContainer {
    width: 100%;
    margin-left: auto;
    margin-right: auto;
    @media only screen and (max-width: 600px) {
      width: 90%;
    }
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
