<template>
  <div class="Mission">
    <v-row>
      <v-col>
        <div class="Mission-wrapper">
          <v-img
            class="Mission-image"
            max-height="1100px"
            max-width="600px"
            src="/shape-11.png"
          />

          <div
            v-observe-visibility="{
              callback: activateAnimationOne,
              once: true,
            }"
          >
            <p class="line1 Mission-title">OUR MISSION IS</p>
            <p class="line2 Mission-title">TO CONNECT,</p>
            <p class="line3 Mission-title">GROW, AND</p>
            <p class="line4 Mission-title">SERVE</p>
          </div>
        </div>
      </v-col>
    </v-row>
    <v-row class="Mission-textContainer">
      <v-col>
        <div
          class="Mission-text"
          v-observe-visibility="{
            callback: activateAnimationTwo,
            once: true,
          }"
        >
          <div>
            <i> CONNECTING TO JESUS AND COMMUNITY, GROWING IN OUR FAITH AND </i>
          </div>
          <div><i> RELATIONSHIPS IN SERVING </i></div>
          <div><i> GOD AND PEOPLE </i></div>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
import anime from 'animejs/lib/anime.es.js'
export default {
  name: 'MissionComponent',
  methods: {
    activateAnimationOne() {
      console.log('Animation 1 Moving')
      // line 1 animation
      anime
        .timeline({
          targets: '.line1',
          translateX: 500,
          direction: 'reverse',
          easing: 'linear',
          duration: 1000,
        })
        .add({ targets: '.line1', color: 'rgba(255,255,255, .1)' }, 0)
      // line 2 animation
      anime
        .timeline({
          targets: '.line2',
          translateX: 500,
          direction: 'reverse',
          easing: 'linear',
          duration: 1500,
        })
        .add({ targets: '.line2', color: 'rgba(255,255,255, .1)' }, 0)
      // line 3 animation
      anime
        .timeline({
          targets: '.line3',
          translateX: 500,
          direction: 'reverse',
          easing: 'linear',
          duration: 2000,
        })
        .add({ targets: '.line3', color: 'rgba(255,255,255, .1)' }, 0)
      // line 4 animations
      anime
        .timeline({
          targets: '.line4',
          translateX: 500,
          direction: 'reverse',
          easing: 'linear',
          duration: 2100,
        })
        .add({ targets: '.line4', color: 'rgba(255,255,255, .1)' }, 0)
    },
    activateAnimationTwo() {
      console.log('Animation 2 Moving')
      anime
        .timeline({
          targets: '.Mission-text',
          translateY: 200,
          direction: 'reverse',
          easing: 'linear',
          duration: 1000,
        })
        .add({ targets: '.Mission-text', color: 'rgba(255,255,255, .1)' }, 0)
    },
  },
}
</script>

<style lang="scss" scoped>
.Mission-wrapper {
  display: flex;
  justify-content: space-between;
}
.Mission-title {
  font-size: 144px;
  font-weight: bold;
  text-align: right;
  line-height: 95.09%;
  margin: 40px 40px 0 0;
  @media only screen and (max-width: 600px) {
    font-size: 40px;
    display: none;
  }
}
.Mission-image {
  margin-top: 50px;
  @media only screen and (max-width: 600px) {
    display: none;
  }
}
.Mission-text {
  font-size: 24px;
  line-height: 28px;
  font-weight: normal;
  margin-left: 35px;
  margin-right: 20px;
}
.Mission-textContainer {
  margin-top: 10px;
}
</style>
