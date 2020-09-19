<template>
  <section id="hero">
    <v-row no-gutters>
      <v-img
        :min-height="'calc(100vh - ' + $vuetify.application.top + 'px)'"
        src="/opener1.jpg"
      >
        <v-theme-provider dark>
          <v-container fill-height>
            <v-row align="center" class="white--text mx-auto" justify="center">
              <v-col class="white--text text-center" cols="12" tag="h1">
                <span
                  :class="[
                    $vuetify.breakpoint.smAndDown ? 'display-1' : 'display-2',
                  ]"
                  class="font-weight-light"
                >
                  WELCOME
                </span>

                <br />

                <span
                  :class="[
                    $vuetify.breakpoint.smAndDown ? 'display-3' : 'display-4',
                  ]"
                  class="font-weight-black"
                >
                  HOME
                </span>
              </v-col>
            </v-row>
          </v-container>
        </v-theme-provider>
      </v-img>
    </v-row>
  </section>
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
