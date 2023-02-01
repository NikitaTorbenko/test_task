<script setup></script>

<template>
  <div class="mars">
    <img class="mars__img" src="../assets/img/mars.png" alt="Mars" />
  </div>
</template>

<style scoped lang="scss">
.mars {
  position: absolute;
  top: 165px;
  right: 50%;

  transform: translateX(50%);

  &__img {
    width: 467px;
    height: 467px;
  }
}
</style>
