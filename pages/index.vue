<template>
  <div>
    <Hero />
    <Sermon />
    <!-- <Mission />
    <Connect /> -->
  </div>
</template>

<script>
import Connect from '../components/PageComponents/HomePage/Connect.vue'
import Mission from '../components/PageComponents/HomePage/Mission.vue'
import Sermon from '../components/PageComponents/HomePage/Sermon.vue'
import Hero from '../components/PageComponents/HomePage/Hero.vue'
export default {
  components: {
    Connect,
    Mission,
    Sermon,
    Hero,
  },
}
</script>
