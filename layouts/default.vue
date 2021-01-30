<template>
  <div>
    <!-- Put Header Component Here -->
    <!-- <head-nav></head-nav> -->

    <v-app>
      <!-- Body of App Goes Here. This shouldn't change -->
      <v-main>
        <nuxt />
      </v-main>

      <!-- Put Footer Component Here -->
      <!-- <foot-bar></foot-bar> -->
    </v-app>
  </div>
</template>

<script>
import HeadNav from '../components/LayoutComponents/HeadNav.vue'
import FootBar from '../components/LayoutComponents/FootBar.vue'
export default {
  components: {
    HeadNav,
    FootBar,
  },
}
</script>
