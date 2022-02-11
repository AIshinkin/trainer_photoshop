<template>
  <div class="header container">
    <div class="header__title">Тренажёр</div>
    <div class="header__select">
      <span class="header__txt">Выбрать меню для запоминания:</span>
      <b-select v-model="chapter">
        <option value="">Все</option>
        <option value="File">File</option>
        <option value="Edit">Edit</option>
        <option value="Image">Image</option>
        <option value="Layer">Layer</option>
        <option value="Type">Type</option>
        <option value="Select">Select</option>
        <option value="Filter">Filter</option>
        <option value="3D">3D</option>
        <option value="View">View</option>
        <option value="Инструменты">Инструменты</option>
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