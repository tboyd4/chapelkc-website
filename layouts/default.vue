<template>
  <div>
    <!-- Put Header Component Here -->
    <head-nav></head-nav>

    <!-- Body of App Goes Here. This shouldn't change -->
    <v-app>
      <v-main>
        <nuxt />
      </v-main>
    </v-app>

    <!-- Put Footer Component Here -->
  </div>
</template>

<script>
import HeadNav from '../components/LayoutComponents/HeadNav.vue'
export default {
  components: {
    HeadNav,
  },
}
</script>
