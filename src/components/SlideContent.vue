<template>
  <div class="comic-card">
    <figure>
      <img :src="thumb" alt="">
    </figure>
    <h3>{{series}}</h3>
  </div>
</template>

<script>
export default {
  props: {
    thumb: String,
    series: String
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