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

          <div class="Mission-title">
            <i>OUR MISSION </i> IS TO CONNECT, GROW, AND SERVE
          </div>
        </div>
      </v-col>
    </v-row>
    <v-row class="Mission-textContainer">
      <v-col>
        <div class="Mission-text">
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
export default {}
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
