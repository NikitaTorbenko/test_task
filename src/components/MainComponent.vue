<script setup>
import LeftSideComponent from '../components/LeftSiddeComponent.vue'
import MarsComponent from '../components/MarsComponent.vue'
import RightSideComponent from '../components/RightSideComponent.vue'

</script>

<template>
    <div class="container">
        <LeftSideComponent/>
        <!-- <MarsComponent/> -->
        <RightSideComponent/> 
    </div>
</template>

<style lang="scss">

.container {
  max-width: 1170px;
  width: 100%;
  margin: 0 auto;

  display: flex;
  justify-content: space-between;
  align-items: center;
}

img { 
  pointer-events: none; 
    -moz-user-select: none; 
    -webkit-user-select: none; 
    -ms-user-select: none; 
    user-select: none;
}

@media (max-width: 1400px) {
  .container {
    width: 960px;
  }
}

@media (max-width: 1200px) {
  .container {
    width: 720px;
  }
}

@media (max-width:726px) {
  .container {
    width: 375px;
    flex-direction: column;
  }
}


</style>