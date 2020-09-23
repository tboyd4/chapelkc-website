<template>
  <div>
    <nav-bar></nav-bar>
    <catcher></catcher>
    <connection-box></connection-box>
    <groups></groups>
  </div>
</template>

<script>
import NavBar from '../components/NavBar.vue'
import Catcher from '../components/Catcher.vue'
import ConnectionBox from '../components/ConnectionBox.vue'
import Groups from '../components/Groups.vue'
export default {
  components: {
    Catcher,
    NavBar,
    ConnectionBox,
    Groups
  }
}
</script>
