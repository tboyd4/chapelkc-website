<template>
  <div class="connect-background">
    <v-row>
      <v-img
        class="connect-background-image"
        :max-height="height"
        :max-width="width"
        src="/connect.png"
      />
    </v-row>
    <div class="my-8"></div>
    <v-row align="center" justify="center">
      <v-col>
        <div class="c-button"><i>Visit</i></div>
      </v-col>
      <v-col>
        <div class="c-button"><i>Connect</i></div>
      </v-col>
      <v-col>
        <div class="c-button"><i>Beliefs</i></div>
      </v-col>
      <v-col>
        <div class="c-button"><i>Give</i></div>
      </v-col>
      <v-col>
        <div class="c-button"><i>Subscribe</i></div>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'ConnectComponent',
  computed: {
    height() {
      switch (this.$vuetify.breakpoint.name) {
        case 'xs':
          return '50px'
        case 'sm':
          return '80px'
        case 'md':
          return '80px'
        case 'lg':
          return '80px'
        case 'xl':
          return '80px'
      }
    },
    width() {
      switch (this.$vuetify.breakpoint.name) {
        case 'xs':
          return '300px'
        case 'sm':
          return '300px'
        case 'md':
          return '900px'
        case 'lg':
          return '900px'
        case 'xl':
          return '900px'
      }
    },
  },
}
</script>

<style>
.connect-background {
  background-color: #f89f9f;
  min-height: 335px;
  padding: 50px;
  margin-top: 30px;
}
.connect-background-image {
  margin-left: 5px;
}
.connect-buttons {
  display: flex;
  justify-content: space-evenly;
  margin-top: 70px;
}
.c-button {
  background-color: white;
  height: 37px;
  width: 183px;
  border: 3px solid #000000;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: auto;
  margin-right: auto;
  font-weight: 700;
  font-size: 36px;
  padding-top: 8px;
  padding-right: 5px;
  cursor: pointer;
}
</style>
