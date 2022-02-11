<template>
  <div class="app">
    <header-page></header-page>
    <banner-page @close="banner = false" v-if="banner"></banner-page>
    <trainer-page></trainer-page>
  </div>
</template>

<script>
import HeaderPage from './components/HeaderPage.vue'
import BannerPage from './components/BannerPage.vue'
import TrainerPage from './components/TrainerPage.vue'

export default {

  data: () => ({
    banner: true,
  }),

  components: {
    HeaderPage,
    BannerPage,
    TrainerPage
  }
}
</script>