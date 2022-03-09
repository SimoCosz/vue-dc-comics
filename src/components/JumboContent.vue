<template>
  <div class="jumbo">
    <div class="container">
      <button class="btn">Current Series</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'JumboContent',
}
</script>

<style lang="scss" scoped>
  .jumbo{
    background-image: url('../assets/img/jumbotron.jpg');
    background-position: top center;
    background-size: cover;
    background-repeat: no-repeat;
    min-height: 250px;
    min-width: 1024px;
    position: relative;

    .btn{
      position: absolute;
      bottom: 0;
      transform: translateY(50%);
      margin: 0 auto;
      padding: 8px 10px;
      border: none;
      background-color: var(--color-blue);
      text-transform: uppercase;
      color: white;
      font-weight: 900;
      cursor: pointer;

      &:hover{
        box-shadow: 2px 2px 5px black;
      }
    }
  }
</style>