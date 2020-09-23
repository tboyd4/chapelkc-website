<template>
  <section id="catcher">
    <v-parallax
      :height="$vuetify.breakpoint.smAndDown ? 700 : 800"
      src="/par1.jpg"
    >
      <v-container fill-height>
        <v-row align="center" class="white--text mx-auto" justify="center">
          <v-col class="black--text text-center" cols="12" tag="h1">
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
    </v-parallax>
    <div class="py-4"></div>

    <v-container class="text-center">
      <h2 class="display-2 font-weight-bold mb-3">VUETIFY FEATURES</h2>

      <v-responsive class="mx-auto mb-12" width="56">
        <v-divider class="mb-1"></v-divider>

        <v-divider></v-divider>
      </v-responsive>

      <v-row>
        <v-col cols="12" md="4">
          <v-card class="py-12 px-4" color="grey lighten-5" flat>
            <h1>Hello</h1>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <div class="py-4"></div>
  </section>
</template>

<script>
export default {}
</script>

<style scoped></style>
