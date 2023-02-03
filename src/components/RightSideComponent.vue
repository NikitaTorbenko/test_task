<script setup></script>

<template>
  <div class="right-side">
    <div class="grid_item gradient-to-right-bottom">
      <span class="grid__text">
        мы<br /><span class="numbers"> 1</span><br />
        на рынке</span
      >
    </div>
    <div class="grid_item gradient-to-left-bottom">
      <span class="grid__text">
        гарантируем<br /><span class="numbers">50%</span><br />
        безопасность</span
      >
    </div>
    <div class="grid_item gradient-to-right-top">
      <span class="grid__text">
        календарик за<br /><span class="numbers">2001</span>г.<br />
        в подарок</span
      >
    </div>
    <div class="grid_item gradient-to-left-top">
      <span class="grid__text">
        путешествие<br /><span class="numbers">597</span><br />
        дней</span
      >
    </div>
  </div>
</template>

<style scoped lang="scss">
.right-side {
  display: grid;
  grid-template-columns: 150px 150px;
  grid-template-rows: 170px 170px;
  grid-gap: 10px;

  margin-top: 120px;
}

.grid_item {
  color: #fff;
  text-align: center;
  line-height: 1.9;
  padding: 8px;

  cursor: pointer;
}

.grid__text {
  font-size: 1rem;
}

.numbers {
  font-size: 3rem;
}

.gradient-to-right-bottom {
  background: linear-gradient(
    to right bottom,
    rgba(255, 255, 255, 0) 50%,
    rgba(255, 255, 255, 0.3) 180%
  );

  transition: all 0.3s; // почему-то не работает

  &:hover {
    background: linear-gradient(
      to right bottom,
      rgba(255, 255, 255, 0) 50%,
      rgba(255, 255, 255, 0.3) 120%
    );

    // border-bottom: 1px solid rgba(200, 200, 200, 0);
    // border-right: 1px solid rgba(255, 255, 255, 0);

    transition: all 0.3s; // почему-то не работает
  }
}

.gradient-to-left-bottom {
  background: linear-gradient(
    to left bottom,
    rgba(255, 255, 255, 0) 50%,
    rgba(255, 255, 255, 0.3) 180%
  );

  &:hover {
    background: linear-gradient(
      to left bottom,
      rgba(255, 255, 255, 0) 50%,
      rgba(255, 255, 255, 0.3) 120%
    );
  }
}

.gradient-to-right-top {
  background: linear-gradient(
    to right top,
    rgba(255, 255, 255, 0) 50%,
    rgba(255, 255, 255, 0.3) 180%
  );

  &:hover {
    background: linear-gradient(
      to right top,
      rgba(255, 255, 255, 0) 50%,
      rgba(255, 255, 255, 0.3) 120%
    );
  }
}

.gradient-to-left-top {
  background: linear-gradient(
    to left top,
    rgba(255, 255, 255, 0) 50%,
    rgba(255, 255, 255, 0.3) 180%
  );

  &:hover {
    background: linear-gradient(
      to left top,
      rgba(255, 255, 255, 0) 50%,
      rgba(255, 255, 255, 0.3) 120%
    );
  }
}

@media (max-width: 726px) {
  .right-side{
    margin-top: 20px;
    grid-template-columns: 134px 134px;
    grid-template-rows: 152px 152px;
    grid-gap: 8px;

  }
  .grid_item {
    line-height: 1.5;

  }
}

@media (max-width: 400px) {
  .right-side{
    margin-top: 18px;
    grid-template-columns: 110px 110px;
    grid-template-rows: 125px 125px;
    grid-gap: 8px;

  }
  .grid_item {
    line-height: 1.6;
  }
.grid__text {
  font-size: .9rem;
}

.numbers {
  font-size: 2rem;
}

}
</style>
