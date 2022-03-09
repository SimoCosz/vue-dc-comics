<template>
  <div class="comic-card">
    <figure>
      <img :src="img" alt="">
    </figure>
    <h3>{{title}}</h3>
  </div>
</template>

<script>
export default {
  props: {
    img: String,
    title: String
  },
}
</script>

<style lang='scss' scoped>
  .comic-card{
    width: calc((100% / 6) - 10px);

    img{
      object-fit: cover;
      object-position: top center;
      aspect-ratio: 1/1;

    }
  }
</style>