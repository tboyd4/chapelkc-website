<template>
  <div>
    <section id="about-me">
      <video class="box1" preload="auto" autoplay loop muted="muted" volume="0">
        <source src="/introclip.mp4" type="video/mp4" />
      </video>
      <section id="features" class="grey lighten-3">
        <v-container class="text-center">
          <v-row>
            <v-col>
              <h2 class="display-1 font-weight-bold mb-3">
                WE WOULD LOVE FOR YOU TO LEARN MORE ABOUT WHO WE ARE
              </h2>
              <v-btn rounded outlined color="#3c92bd">Click Here!</v-btn>
            </v-col>
          </v-row>
        </v-container>
      </section>
    </section>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.box1 {
  width: 100% !important;
  height: 450px !important;
  object-fit: cover;
}
</style>
