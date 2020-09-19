<template>
  <div>
    <nav-bar></nav-bar>
    <catcher></catcher>
    <video-sermon></video-sermon>
  </div>
</template>

<script>
import NavBar from '../components/NavBar.vue'
import Catcher from '../components/Catcher.vue'
import VideoSermon from '../components/VideoSermon.vue'
export default {
  components: {
    Catcher,
    VideoSermon,
    NavBar
  }
}
</script>
