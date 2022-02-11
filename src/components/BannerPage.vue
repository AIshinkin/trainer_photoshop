<template>
  <div class="banner container">
    <div class="banner__logo">
      <img class="banner__logo-img" src="../assets/banner.png" alt="">
    </div>
    <div class="banner__info">
      <h2 class="banner__info-title">Внимание!</h2>
      <p>Данный инструмент разработан для заучивания пунктов меню программы и их функциональности.</p>
      <p>Все совпадения случайны, инструмент разработан на полном энтузиазме :)</p>
      <p>
        <b-button type="is-success" @click="$emit('close')">Понятно, спасибо :)</b-button>
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.banner {
  display: flex;
  justify-content: center;

  &__logo {
    text-align: right;
    padding-right: 20px;

    &-img {
      width: 80%;
    }
  }

  &__info {
    &-title {
      font-size: 30px;
      font-weight: bold;
    }
    
    p {
      margin-top: 15px;
    }
  }
}
</style>