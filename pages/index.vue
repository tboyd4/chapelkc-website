<template>
  <div>
    <!-- section 1 HERO SECTION -->
    <div>
      <v-img
        class="hero-image"
        max-height="300px"
        max-width="675px"
        src="/this-is-home.png"
      />
      <div class="hero-title"><i>CONNECT.GROW.SERVE</i></div>
    </div>
    <!-- section 2 SERMON SECTION -->
    <div>
      <div class="sermon-title">LASTEST SERMON:</div>
      <div class="sermon-subtitle">VISION CORRECTION</div>
      <video width="100%" height="653" controls>
        <source src="introclip.mp4" type="video/mp4" />
        Your browser does not support the video tag.
      </video>
    </div>
    <!-- section 3 MISSION SECTION -->
    <div>
      <div class="mission-wrapper">
        <v-img
          class="mission-image"
          max-height="1100px"
          max-width="600px"
          src="/shape-11.png"
        />
        <div class="mission-title">
          <i>OUR MISSION </i> IS TO CONNECT, GROW, AND SERVE
        </div>
      </div>
      <div class="mission-text">
        <div>
          <i> CONNECTING TO JESUS AND COMMUNITY, GROWING IN OUR FAITH AND </i>
        </div>
        <div><i> RELATIONSHIPS IN SERVING </i></div>
        <div><i> GOD AND PEOPLE </i></div>
      </div>
    </div>
    <ConnectComponent />
  </div>
</template>

<script>
import ConnectComponent from '../components/PageComponents/HomePage/ConnectComponent.vue'
export default {
  components: {
    ConnectComponent,
  },
}
</script>

<style lang="scss" scoped>
.hero-image {
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-top: 200px;
  width: 50%;
}
.hero-title {
  font-size: 36px;
  line-height: 41.4px;
  text-align: center;
  margin-top: 60px;
}
.sermon-title {
  font-size: 64px;
  font-weight: 700;
  line-height: 73.59px;
  text-align: left;
  margin: 200px 0 0 35px;
}
.sermon-subtitle {
  font-style: normal;
  font-weight: normal;
  font-size: 48px;
  line-height: 55px;
  margin: 0 0 35px 35px;
}
.mission-wrapper {
  display: flex;
  justify-content: space-between;
}
.mission-title {
  font-size: 144px;
  font-weight: bold;
  text-align: right;
  line-height: 95.09%;
  margin: 40px 40px 0 0;
}
.mission-image {
  margin-top: 50px;
}
.mission-text {
  font-size: 24px;
  line-height: 28px;
  font-weight: normal;
  margin-left: 35px;
}
</style>
