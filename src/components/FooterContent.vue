<template>
  <div class="footer">
    <div class="container">
      <div class="list">
        <ul>
          <li v-for="(el, i) in footerMenu" :key='i' class="item-wrap">
            <h4 class="title">{{el.title}}</h4> 
            <ul>
              <li v-for='(link, i) in el.links' :key='i' class="item">
                <a :href="link.href">{{link.text}}</a>
              </li>
            </ul>
          </li>
        </ul>
      </div>
      <div class="logo-wrapper">
        <img class="logo-bg" src="../assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
    
    <div class="social-banner">
      <div class="social">
      <button>Sign up now</button>
      <div class="social-link">
      <span>Follow US</span>
        <ul class="icon-wrap">
          <li v-for="(el, i) in socialIcon" :key="i">
            <a href=""><img :src="require(`../${el.icon}`)" alt=""></a>
          </li>
        </ul>
      </div>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'FooterContent',

  data() {
    return {
      footerMenu: [
        {
          title: 'DC comics',
          links: [
            {
              text: 'Character',
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
              text: 'TV',
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
        },

        {
          title: 'Shop',
          links: [
            {
            text: 'Shop DC',
            href: '#'
            },
            {
            text: 'Shop DC Collectibles',
            href: '#'
            },
          ],
        },

        {
          title: 'DC',
          links: [
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
              text: 'Talent Workshops',
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
        },

        {
          title: 'Sites',
          links: [
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
          ],
        }
      ],
      socialIcon: [
        {
          icon: 'assets/img/footer-facebook.png'
        },
        {
          icon: 'assets/img/footer-twitter.png'
        },
        {
          icon: 'assets/img/footer-youtube.png'
        },
        {
          icon: 'assets/img/footer-pinterest.png'
        },
        {
          icon: 'assets/img/footer-periscope.png'
        },
      ]



    }
  }
}
</script>

<style lang='scss' scoped>

  .footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    position: relative;



    .container{
      color: white;
      height: 450px;
      display: flex;
      justify-content: space-between;
      gap: 40px;
      position: relative;

      .logo-wrapper{
        width: 450px;
        height: 450px;
        object-fit: cover;
      }

      .list{
        max-height: 100%;
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        margin-top: 40px;

        .item-wrap{
          padding: 20px;
        }

        .title{
          font-weight: 800;
          margin: 10px 0;
          text-transform: uppercase;
        }

        .item{
          color: #aaa;
          font-size: 12px;
        }
      }

      ul{
        display: contents;
      }
    }

    .social-banner{
      position: absolute;
      bottom: 0;
      height: 80px;
      width: 100%;
      padding: 20px;
      background-color: var(--color-black);

      .social{
        display: flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        margin: 0 auto;
        width: 1024px;

        button{
          background-color: transparent;
          border: 2px solid var(--color-blue);
          padding: 10px;
          color: white;
          text-transform: uppercase;
          font-weight: 800;
        }

        .social-link{
          display: flex;
          align-items: center;
          gap: 20px;

          .icon-wrap{
            display: flex;
            gap: 20px;
            padding: 20px 10px;

            img{
            object-fit: contain;
            }
          }

          span{
            text-transform: uppercase;
            font-weight: 900;
            color: var(--color-blue);
          }
        }

      }

    }
  }


</style>