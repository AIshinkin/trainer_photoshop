<template>
  <div class="header container">
    <div class="header__title">Тренажёр</div>
    <div class="header__select">
      <span class="header__txt">Выбрать меню для запоминания:</span>
      <b-select v-model="chapter">
        <option value="">Все</option>
        <option value="silver">Silver</option>
      </b-select>
    </div>
  </div>
</template>


<script>
export default {
  data: () => ({
    chapter: '',
  })
}
</script>



<style lang="scss" scoped>
.header {
  display: flex;
  justify-content: space-between;
  aling-items: center;
  padding: 20px 0;

  &__title {
    font-size: 20px;
  }

  &__select {
    display: flex;
    align-items: center;
  }

  &__txt {
    margin-right: 15px;
  }
}
</style>