<template>
  <div id="app">
    <!-- Header -->
    <HeaderContent />
    <!-- Main -->
    <MainContent />
    <!-- Footer -->
    <FooterContent />
  </div>
</template>

<script>
import HeaderContent from './components/HeaderContent.vue'
import MainContent from './components/MainContent.vue'
import FooterContent from './components/FooterContent.vue'

export default {
  name: 'App',
  components: {
    HeaderContent,
    MainContent,
    FooterContent
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
