<template>
  <div id="app">
    <!-- Header -->
    <HeaderContent />
    <!-- Main -->
    <MainContent />
    <MainBanner />
    <!-- Footer -->
    <FooterContent />
  </div>
</template>

<script>
import HeaderContent from './components/HeaderContent.vue'
import MainContent from './components/MainContent.vue'
import FooterContent from './components/FooterContent.vue'
import MainBanner from './components/MainBanner.vue'

export default {
  name: 'App',
  components: {
    HeaderContent,
    MainContent,
    MainBanner,
    FooterContent,
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container{
  width: 1024px;
  margin: 0 auto;
}

a{
  text-decoration: none;
  color: currentColor;
}

ul {
  list-style: none;
}

img{
  width: 100%;
  height: 100%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  --color-blue: #0482F9;
  --color-black: #4C4646;
  
}
</style>
