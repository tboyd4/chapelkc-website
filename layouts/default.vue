<template>
  <div>
    <v-app>
      <v-main>
        <nuxt />
      </v-main>
    </v-app>

    <v-footer class="justify-center" color="white" height="100">
      <div
        class="font-weight-light white--text text--white text-center mx-auto"
      >
        &copy; {{ new Date().getFullYear() }} — The Chapel KC
      </div>
    </v-footer>
  </div>
</template>

<script>
export default {}
</script>
