<template>
  <v-card class="mx-auto overflow-hidden">
    <v-app-bar app flat color="#FFFFFF">
      <v-img max-height="45px" max-width="45px" src="/TCKCLogo1.png" />
      <v-spacer></v-spacer>
      <div>
        <v-btn text color="primary" class="ma-6 px-1 py-1">About Us</v-btn>
        <v-btn text color="primary" class="ma-6 px-1 py-1">Next Steps</v-btn>
        <v-btn text color="primary" class="ma-6 px-1 py-1">Give</v-btn>
        <v-btn text color="primary" class="ma-6 px-1 py-1">Messages</v-btn>
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
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>

          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Account</v-list-item-title>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>
  </v-card>
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

<style></style>
