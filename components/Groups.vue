<template>
  <section id="stats">
    <v-parallax
      :height="$vuetify.breakpoint.smAndDown ? 700 : 800"
      src="/par2.jpg"
    >
      <v-container fill-height>
        <v-row class="mx-auto">
          <v-col v-for="[value, title] of stats" :key="title" cols="12" md="3">
            <div class="text-center">
              <div
                class="display-3 font-weight-black mb-4"
                v-text="value"
              ></div>

              <div
                class="title font-weight-regular text-uppercase"
                v-text="title"
              ></div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </v-parallax>
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
  </section>
</template>

<script>
export default {}
</script>

<style scoped></style>
