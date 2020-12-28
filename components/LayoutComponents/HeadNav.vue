<template>
  <v-card class="mx-auto overflow-hidden">
    <v-app-bar app flat color="#FFFFFF">
      <v-img max-height="48px" max-width="48px" src="/TCKCLogo1.png" />
      <v-spacer></v-spacer>
      <div :v-if="!isMobileScreen">
        <v-btn
          text
          color="primary"
          class="d-none d-md-inline ma-6 px-1 py-1"
          to="/"
          >Home</v-btn
        >
        <v-btn
          text
          color="primary"
          class="d-none d-md-inline ma-6 px-1 py-1"
          to="/about-us"
          >About Us</v-btn
        >
        <v-btn
          text
          color="primary"
          class="d-none d-md-inline ma-6 px-1 py-1"
          to="/next-steps"
          >Next Steps</v-btn
        >
        <v-btn
          text
          color="primary"
          class="d-none d-md-inline ma-6 px-1 py-1"
          to="/give"
          >Give</v-btn
        >
        <v-btn
          text
          color="primary"
          class="d-none d-md-inline ma-6 px-1 py-1"
          to="/messages"
          >Messages</v-btn
        >
      </div>
      <v-spacer></v-spacer>
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
    </v-app-bar>

    <v-navigation-drawer app v-model="drawer" absolute right temporary>
      <v-list nav dense>
        <v-list-item-group
          v-model="group"
          active-class="deep-purple--text text--accent-4"
        >
          <v-list-item to="/">
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>

          <v-list-item to="/about-us">
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-title>About Us</v-list-item-title>
          </v-list-item>

          <v-list-item to="/next-steps">
            <v-list-item-icon>
              <v-icon>mdi-chevron-right-box</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Next Steps</v-list-item-title>
          </v-list-item>

          <v-list-item to="/give">
            <v-list-item-icon>
              <v-icon>mdi-email</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Give</v-list-item-title>
          </v-list-item>

          <v-list-item to="/messages">
            <v-list-item-icon>
              <v-icon class="px-2">mdi-book-arrow-down</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Messages</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </v-card>
</template>

<script>
export default {
  mounted() {
    if (
      this.$vuetify.breakpoint === 'xs' ||
      this.$vuetify.breakpoint === 'sm'
    ) {
      this.isMobileScreen = true
    }
  },
  data: () => {
    return {
      isMobileScreen: false,
      drawer: false,
      group: null,
    }
  },
}
</script>

<style></style>
