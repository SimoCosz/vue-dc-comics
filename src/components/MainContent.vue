<template>
<main class="main">
  <div class="container">
    <div class="content">
      {{text}}
    </div>
  </div>
    <div class="banner">
      <MainBanner />
    </div>
</main>
</template>

<script>
import MainBanner from '../components/MainBanner.vue'

export default {
  name: 'MainContent',
  components: {
    MainBanner,
  },

  data() {
    return {
      text: '--> Content gose here <---'
    }
  }
}
</script>

<style lang='scss' scoped>

  .main{
    background-color: var(--color-black);
    height: 70px;
    margin: 0 auto;

    .container{
      height: 100%;
      display: flex;
      align-items: center;
    }
    
    .content{
      color: white;
      font-weight: 900;
    }
  }

</style>