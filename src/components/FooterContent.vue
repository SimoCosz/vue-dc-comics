<template>
  <div class="footer">
    <div class="container">
      <div class="list">
        <h4 class="title">Dc comics</h4> 
        <ul>
          <li v-for='(link, i) in links' :key='i' class="item">
            <a :href="link.href">{{link.text}}</a>
          </li>
        </ul>
        <h4 class="title">Shop</h4> 
        <ul>
          <li v-for='(link, i) in links2' :key='i' class="item">
            <a :href="link.href">{{link.text}}</a>
          </li>
        </ul>
      </div>
      <div class="list">
        <h4 class="title">Dc</h4> 
        <ul>
          <li v-for='(link, i) in links3' :key='i' class="item">
            <a :href="link.href">{{link.text}}</a>
          </li>
        </ul>
      </div>
      <div class="list">
        <h4 class="title">Sites</h4> 
        <ul>
          <li v-for='(link, i) in links4' :key='i' class="item">
            <a :href="link.href">{{link.text}}</a>
          </li>
        </ul>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'FooterContent',

  data() {
    return {
      links: [
        {
          text: 'character',
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
          text: 'Videos',
          href: '#'
        },
        {
          text: 'News',
          href: '#'
        },
      ],

      links2:[
        {
          text: 'Shop DC',
          href: '#'
        },
        {
          text: 'Sho DC Collectibles',
          href: '#'
        },
      ],

      links3: [
        {
          text: 'Terms Of Use',
          href: '#'
        },
        {
          text: 'Privacy policy (New)',
          href: '#'
        },
        {
          text: 'Ad Choices',
          href: '#'
        },
        {
          text: 'Advertising',
          href: '#'
        },
        {
          text: 'Jobs',
          href: '#'
        },
        {
          text: 'Subscriptions',
          href: '#'
        },
        {
          text: 'Talent Worshops',
          href: '#'
        },
        {
          text: 'CPSC Certificates',
          href: '#'
        },
        {
          text: 'Ratings',
          href: '#'
        },
        {
          text: 'Shop Help',
          href: '#'
        },
        {
          text: 'Contact Us',
          href: '#'
        },
      ],
      links4: [
        {
          text: 'DC',
          href: '#'
        },
        {
          text: 'MAD Magazine',
          href: '#'
        },
        {
          text: 'DC Kids',
          href: '#'
        },
        {
          text: 'DC Universe',
          href: '#'
        },
        {
          text: 'DC Power Visa',
          href: '#'
        },
      ]
    }
  }
}
</script>

<style lang='scss' scoped>

  .footer{
    background-image: url('../assets/img/footer-bg.jpg');

    .container{
      color: white;
      height: 400px;
      padding-top: 40px;
      display: flex;
      gap: 40px;
      text-transform: uppercase;

      .title{
        font-weight: 800;
        margin: 10px 0;

      }

      .item{
        color: #aaa;
        font-size: 12px;
      }
    }
  }


</style>