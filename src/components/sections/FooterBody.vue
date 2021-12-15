<template>
  <footer>
    <section class="footer-body">
      <div class="container">
      <img src="../../assets/img/dc-logo-bg.png" alt="DC Logo" id="logo-footer">
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
    </section>
  </footer>
</template>

<script>


export default {
  name: 'FooterBody',
  data() {
    return {
      
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



  .footer-body {
    background-image: url('../../assets/img/footer-bg.jpg');
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
            margin: 8px 0;
            a {
              color: #777;
              text-decoration: none;
              font-size: 14px;
            }  
          }
        }
      }
    }
    }
    
  }

  


</style>
