<template>
  <footer>
    <div class="footer-top">
      <div class="container">
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :href="link.url">
              <img :src="require(`../assets/img/${link.img}`)" :alt="link.text">
              {{link.text}}
            </a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data() {
    return {
      links: [
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
  }

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
          @include flex-center;
          img {
            margin-right: 15px;
            height: 40px;
          }
        }
      }
    }
  }


</style>
