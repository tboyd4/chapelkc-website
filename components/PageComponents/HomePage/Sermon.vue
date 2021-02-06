<template>
  <div class="SermonVideo">
    <v-row>
      <div class="SermonVideo-title">LASTEST SERMON:</div>
    </v-row>
    <v-row>
      <v-col>
        <div class="SermonVideo-subTitle">VISION CORRECTION</div>
      </v-col>
    </v-row>
    <v-row align="center" justify="center">
      <v-col cols="12">
        <div>
          <video class="SermonVideo-player" :height="height" controls>
            <source src="sample.mp4" type="video/mp4" />
            Your browser does not support the video tag.
          </video>
        </div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  computed: {
    height() {
      switch (this.$vuetify.breakpoint.name) {
        case 'xs':
          return 350
        case 'sm':
          return 475
        case 'md':
          return 700
        case 'lg':
          return 850
        case 'xl':
          return 1200
      }
    },
  },
}
</script>

<style lang="scss" scoped>
.SermonVideo {
  margin-top: 300px;
  .SermonVideo-title {
    margin-left: 25px;
    font-family: Helvetica;
    font-style: normal;
    font-weight: bold;
    font-size: 64px;
    line-height: 74px;
  }
  .SermonVideo-subTitle {
    margin-left: 25px;
    font-family: Helvetica;
    font-style: normal;
    font-weight: normal;
    font-size: 48px;
    line-height: 55px;
  }
  .SermonVideo-player {
    width: 100%;
    z-index: -100;
    object-fit: fill;
  }
}
</style>
