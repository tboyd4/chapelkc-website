<template>
  <div>
    <nav-bar></nav-bar>
    <catcher></catcher>
    <video-sermon></video-sermon>
    <connection-box></connection-box>
  </div>
</template>

<script>
import NavBar from '../components/NavBar.vue'
import Catcher from '../components/Catcher.vue'
import VideoSermon from '../components/VideoSermon.vue'
import ConnectionBox from '../components/ConnectionBox.vue'
export default {
  components: {
    Catcher,
    VideoSermon,
    NavBar,
    ConnectionBox
  }
}
</script>
