<template>
  <div class="main-banner">
    <div class="container">
      <ul>
        <li v-for='(link, i) in links' :key='i' class="item">
          <img :src="link.image" alt="">
          <a :href="link.href">{{link.text}}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'MainBanner',

    data() {
      return {
        links: [
          {
            image: '../assets/img/buy-comics-digital-comics.png',
            text: 'Digital comics',
            href: '#'
          },
          {
            image: '../assets/img/buy-comics-merchandise.png',
            text: 'Dc merchendise',
            href: '#'
          },
          {
            image: '../assets/img/buy-comics-subscriptions.png',
            text: 'Subscription',
            href: '#'
          },
          {
            image: '../assets/img/buy-comics-shop-locator.png',
            text: 'Comic shop locator',
            href: '#'
          },
          {
            image: '../assets/img/buy-comics-power-visa.svg',
            text: 'Dc power visa',
            href: '#'
          },
        ]
      }
    }
  }  
</script>

<style lang="scss" scope>
  .main-banner{
    background-color: var(--color-blue);

    .container{
      display: flex;
      justify-content: space-between;
      align-items: center;

      ul{
        display: contents;
        list-style: none;
      }

      .item{
        padding: 0 20px;

        .image{
          width: 30px;
        }

      }
    }
  }
</style>