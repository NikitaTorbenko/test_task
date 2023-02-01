<script setup></script>

<template>
  <header class="header">
    <div class="container flex-container">
      <div class="logo">
        <img src="../assets/img/logo.png" alt="SPASE_X" />
      </div>

      <nav>
        <ul class="menu">
          <li class="menu__item"><a href="#" class="menu__link">Главная</a></li>
          <li class="menu__item">
            <a href="#" class="menu__link">Технология</a>
          </li>
          <li class="menu__item">
            <a href="#" class="menu__link">График полетов</a>
          </li>
          <li class="menu__item">
            <a href="#" class="menu__link">Гарантии</a>
          </li>
          <li class="menu__item">
            <a href="#" class="menu__link">О компании</a>
          </li>
          <li class="menu__item">
            <a href="#" class="menu__link">Контакты</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style scoped lang="scss">
.container {
  max-width: 1170px;
  width: 100%;
  margin: 0 auto;
}

.header {
  border: 1px solid rgba(255, 255, 255, 0.2);
  height: 100px;
}

.logo {
  height: 100px;
}

.flex-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.menu {
  display: flex;

  &__item {
    margin-left: 25px;
  }

  &__link {
    color: rgba(255, 255, 255, 0.8);
    text-decoration: none;

    position: relative;

    transition: .3s;

    &::after {
        content: "";
        display: block;
        position: absolute;
        top: 140%;
        left: 50%;
        height: 1px;
        width: 0;
        background-color: rgba(255, 255, 255, 0.6);
        transition: .3s;

    }

    &:hover::after {
        width: 100%;
        left: 0;
    }

    &:hover {
        color: rgba(255, 255, 255, 0.6)
    }
  }
}
</style>
