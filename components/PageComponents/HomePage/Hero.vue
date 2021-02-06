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
export default {
  methods: {},
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
