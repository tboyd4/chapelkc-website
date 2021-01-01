<template>
  <div class="connect-background">
      <v-img class="connect-background-image" max-height="80px" max-width="900px" src="/connect.png" />
      <div class="connect-buttons">
        <div class="c-button"><i>Visit</i> </div>
        <div class="c-button"><i>Connect</i> </div>
        <div class="c-button"><i>Beliefs</i> </div>
        <div class="c-button"><i>Give</i> </div>
        <div class="c-button"><i>Subscribe</i> </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'ConnectComponent'
}
</script>

<style>
.connect-background{
    background-color: #F89F9F;
    min-height: 335px;
    padding: 50px;
    margin-top: 30px;
}
.connect-background-image{
margin-left: 5px;
}
.connect-buttons{
display: flex;
justify-content: space-evenly;
margin-top: 70px;
}
.c-button{
background-color: white;
height: 37px;
width: 183px;
border: 3px solid #000000;
display: flex;
justify-content: center;
align-items: center;
font-weight: 700;
font-size: 36px;
line-height: 41.4px;
padding-top:8px;
padding-right: 5px;
cursor: pointer;
}
</style>