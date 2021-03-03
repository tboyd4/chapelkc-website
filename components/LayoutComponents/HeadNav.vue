<template>
  <div>
    <v-app-bar app absolute flat color="#FFFFFF">
      <v-img max-height="48px" max-width="48px" src="/TCKCLogo1.png" />
      <v-spacer></v-spacer>
      <div class="navigation-buttons">
        <v-btn
          text
          color="primary"
          class="nav-button d-none d-md-inline ma-6 px-1 py-1"
          to="/"
          >Home</v-btn
        >
        <v-btn
          text
          color="primary"
          class="nav-button d-none d-md-inline ma-6 px-1 py-1"
          to="/about-us"
          >About Us</v-btn
        >
        <v-btn
          text
          color="primary"
          class="nav-button d-none d-md-inline ma-6 px-1 py-1"
          to="/next-steps"
          >Next Steps</v-btn
        >
        <v-btn
          text
          color="primary"
          class="nav-button d-none d-md-inline ma-6 px-1 py-1"
          to="/give"
          >Give</v-btn
        >
        <v-btn
          text
          color="primary"
          class="nav-button d-none d-md-inline ma-6 px-1 py-1"
          to="/messages"
          >Messages</v-btn
        >
      </div>
      <v-spacer></v-spacer>
      <!-- <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon> -->
    </v-app-bar>

    <!-- <v-navigation-drawer app v-model="drawer" absolute right temporary>
      <v-list nav>
        <v-list-item-group v-model="group">
          <v-list-item to="/">
            <v-list-item-icon class="nav-icon">
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>

          <v-list-item to="/about-us">
            <v-list-item-icon class="nav-icon">
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-title>About Us</v-list-item-title>
          </v-list-item>

          <v-list-item to="/next-steps">
            <v-list-item-icon class="nav-icon">
              <v-icon>mdi-chevron-right-box</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Next Steps</v-list-item-title>
          </v-list-item>

          <v-list-item to="/give">
            <v-list-item-icon class="nav-icon">
              <v-icon>mdi-email</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Give</v-list-item-title>
          </v-list-item>

          <v-list-item to="/messages">
            <v-list-item-icon class="nav-icon">
              <v-icon class="px-2">mdi-book-arrow-down</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Messages</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer> -->
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      drawer: false,
      group: null,
    }
  },
}
</script>

<style lang="scss" scoped>
.nav-button {
  margin-left: 20px;
  margin-right: 20px;
  font-weight: bold;
  font-family: Helvetica, Helvetica, sans-serif;
}
.nav-icon {
  margin-right: 3px;
}
.navigation-buttons {
  @media only screen and (max-width: 600px) {
    display: none;
  }
}
</style>
