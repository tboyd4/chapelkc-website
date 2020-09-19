<template>
  <div>
    <section id="about-me">
        <video class="box1" preload="auto" autoplay loop muted="muted" volume="0">
          <source src="/introclip.mp4" type="video/mp4" />
        </video>
    </section>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.box1 {
  width: 100% !important;
  height: auto !important;
  object-fit: fill;
}
</style>
