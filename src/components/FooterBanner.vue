<template>
  <footer class="banner">
    <div class="container">
      <nav class="list">
        <ul>
          <li v-for='(link, i) in links' :key='i' class="item">
            <a :href="link.href">{{link.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterBanner',

  data() {
    return {

    links: [
      {
        text: 'Characters',
        href: '#'
      },
      {
        text: 'Comics',
        href: '#'
      },
      {
        text: 'Movies',
        href: '#'
      },
      {
        text: 'Tv',
        href: '#'
      },
      {
        text: 'Games',
        href: '#'
      },
      {
        text: 'Collectibles',
        href: '#'
      },
      {
        text: 'Videos',
        href: '#'
      },
      {
        text: 'Fans',
        href: '#'
      },
      {
        text: 'News',
        href: '#'
      },
      {
        text: 'Shop',
        href: '#'
      },

    ]
    }
  },

}
</script>

<style lang='scss' scoped>

  .container{
    padding: 10px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .list{
      display: flex;
      gap: 20px;
      font-size: 10px;

      a{
        text-decoration: none;
        text-transform: uppercase;
        color: var(--color-black);
        font-weight: 800;
        padding: 100% 0;

        &.active{
          color: var(--color-blue);
          border-bottom: 5px solid var(--color-blue);
        }
      }
    }

    ul{
      display: contents;
      list-style: none;
    }
  }

</style>