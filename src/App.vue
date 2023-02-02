<script setup>
import HeaderComponent from "../src/components/HeaderComponent.vue";
import MainComponent from "../src/components/MainComponent.vue";

</script>

<template>
  <div class="wrap">
    <HeaderComponent />
    <MainComponent />
  </div>
</template>

<style lang="scss">
@import "./_global_reset.css";

.wrap {
  width: 100%;
  height: 100vh;

  font-family: 'Roboto', sans-serif;
  
  // background: url(../src/assets/img/background.jpg) 0 0/100% auto no-repeat;;
  background-image: url(../src/assets/img/background.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  // background-size: contain;
  background-position: center bottom;
}

</style>
