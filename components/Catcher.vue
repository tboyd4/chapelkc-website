<template>
  <div>
    <!-- <v-row no-gutters>
      <v-container fill-height>
        <v-row class="my-16" justify="center" align="center">
          <v-col cols="10" md="8">
            <div class="header-box">
              <v-responsive align="center"
                ><span class="header text-center text-h3 text-md-h1 pt-12"
                  >Welcome Home.</span
                ></v-responsive
              >
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-row> -->

    <section id="catch">
      <v-parallax
        :height="$vuetify.breakpoint.smAndDown ? 500 : 1100"
        src="/stock1.jpg"
      >
        <v-container fill-height>
          <v-row class="mx-auto">
            <v-col cols="12" md="3">
              <span class="header text-center text-h3 text-md-h1 pt-12"
                >Welcome Home.</span
              >
            </v-col>
          </v-row>
        </v-container>
      </v-parallax>
    </section>

    <video playsinline autoplay muted loop width="100%">
      <source src="/introclip.mp4" type="video/mp4" />
      <span class="text--white text-center text-h5 text-md-h3 pt-12">Latest Sermon</span>
    </video>

  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.header {
  font-weight: 900;
  font-size: 120px;
}
.header-box {
  height: 900px;
}
</style>
