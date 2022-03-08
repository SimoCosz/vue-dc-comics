<template>
<main class="main">
  <div class="container">
    <div class="content">
      {{text}}
    </div>
  </div>
</main>
</template>

<script>

export default {
  name: 'MainContent',

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