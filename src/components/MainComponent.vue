<script setup>
import LeftSideComponent from '../components/LeftSiddeComponent.vue'
import MarsComponent from '../components/MarsComponent.vue'
import RightSideComponent from '../components/RightSideComponent.vue'



</script>

<template>
    <div class="container">
        <LeftSideComponent/>
        <MarsComponent/>
        <RightSideComponent/> 
    </div>
</template>

<style scoped lang="scss">

.container {
  max-width: 1170px;
  width: 100%;
  margin: 0 auto;

  display: flex;
  justify-content: space-between;
  align-items: center;
}

</style>