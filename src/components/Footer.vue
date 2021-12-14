<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <ul>
          <li v-for="(link, index) in linksFooterTop" :key="index">
            <a :href="link.url">
              <img :src="require(`../assets/img/${link.img}`)" :alt="link.text">
              {{link.text}}
            </a>
          </li>
        </ul>
      </div>
    </div>
    <div class="footer-body">
      <div class="container">
      <img src="../assets/img/dc-logo-bg.png" alt="DC Logo" id="logo-footer">
        <div class="container-list">
          <div class="lista" v-for="(obj, index) in linksFooterBody" :key="index">
            <h2>{{obj.title}}</h2>
            <ul>
              <li v-for="(link, j) in obj.links" :key="j">
                <a :href="link.url">{{link.name}}</a>
              </li>
            </ul>
          </div>
      
        </div>

      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      linksFooterTop: [
        {
          text: "digital comics",
          url: "#",
          img: 'buy-comics-digital-comics.png',
        },
        {
          text: "dc merchandise",
          url: "#",
          img: 'buy-comics-merchandise.png',
        },
        {
          text: "subscription",
          url: "#",
          img: 'buy-comics-subscriptions.png',
        },
        {
          text: "comic shop locator",
          url: "#",
          img: 'buy-comics-shop-locator.png',
        },
        {
          text: "dc pawer visa",
          url: "#",
          img: 'buy-dc-power-visa.svg',
        },
      ],
      linksFooterBody: [
        {
          title: 'dc comics',
          links: [
            {
              name: 'Characters',
              url: '#'
            },
            {
              name: 'Comics',
              url: '#'
            },
            {
              name: 'Movies',
              url: '#'
            },
            {
              name: 'Tv',
              url: '#'
            },
            {
              name: 'Games',
              url: '#'
            },
            {
              name: 'Videos',
              url: '#'
            },{
              name: 'News',
              url: '#'
            }
          ]
        },
        {
          title: 'shop',
          links: [
            {
              name: 'Shop DC',
              url: '#'
            },
            {
              name: 'Shop DC Collectibles',
              url: '#'
            }
          ]
        },
        {
          title: 'dc',
          links: [
            {
              name: 'Termes Of Use',
              url: '#'
            },
            {
              name: 'Privacy policy (New)',
              url: '#'
            },
            {
              name: 'Ad Choices',
              url: '#'
            },
            {
              name: 'Advertising',
              url: '#'
            },
            {
              name: 'Jobs',
              url: '#'
            },
            {
              name: 'Subscriptions',
              url: '#'
            },
            {
              name: 'Talent Workshops',
              url: '#'
            },
            {
              name: 'CPSC Certificates',
              url: '#'
            },
            {
              name: 'Ratings',
              url: '#'
            },
            {
              name: 'Shop Help',
              url: '#'
            },
            {
              name: 'Contact Us',
              url: '#'
            }
          ]
        },
        {
          title: 'sites',
          links: [
            {
              name: 'DC',
              url: '#'
            },
            {
              name: 'MAD Magazine',
              url: '#'
            },
            {
              name: 'DC Kids',
              url: '#'
            },
            {
              name: 'DC Universe',
              url: '#'
            },
            {
              name: 'DC Power Visa',
              url: '#'
            },
          ]
        },
      ]

    }
  }
}
</script>

<style scoped lang="scss">

  @import '../assets/style/partials/mixins.scss';
  @import '../assets/style/partials/variables.scss';

  .footer-top {
    background-color: $dc-blue;
    height: 130px;
    .container {
      height: 100%;
      ul {
        display: flex;
        align-items: center;
        justify-content: space-between;
        list-style: none;
        height: 100%;
        li {
        height: 100%;
          a {
            color: white;
            height: 100%;
            display: flex;
            text-transform: uppercase;
            text-decoration: none;
            font-size: 14px;
            @include flex-center;
            img {
              margin-right: 15px;
              height: 40px;
            }
          }
        }
      }
    }
  }

  .footer-body {
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    .container {
    position: relative;
    overflow: hidden;
      > img {
      position: absolute;
      right: 0;
      top: 50%;
      transform: translateY(-50%);
      }
      .container-list {
      padding: 40px 0;
      display: flex;
      .lista {
        display: inline-block;
        margin-right: 35px;
        color: white;
        h2 {
          margin: 15px 0;
          text-transform: uppercase;
        }
        ul {
          list-style: none;
          li {
            margin: 10px 0;
            a {
              color: #777;
              text-decoration: none;
            }  
          }
        }
      }
    }
    }
    
  }

  


</style>
