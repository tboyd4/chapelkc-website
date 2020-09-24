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
      <h2 class="display-2 font-weight-bold mb-3">WHO WE ARE</h2>

      <v-responsive class="mx-auto mb-12" width="56"> </v-responsive>

      <v-row>
        <v-col v-for="(card, index) in cardinfo" :key="index" cols="12" md="4">
          <v-card outlined>
            <v-list-item three-line>
              <v-list-item-content>
                <div class="overline mb-4">{{ card.over }}</div>
                <v-list-item-title class="headline py-4"
                  >{{ card.text }}</v-list-item-title
                >
              </v-list-item-content>
            </v-list-item>

          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <div class="py-4"></div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      cardinfo: [
        { text: 'Something about our church.', over: 'US' },
        { text: 'Something about our mission.', over: 'MISSION' },
        { text: 'Something about our God', over: 'HIM' },
      ],
    }
  },
}
</script>

<style scoped></style>
