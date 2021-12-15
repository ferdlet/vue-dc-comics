<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="../../assets/img/dc-logo.png" alt="Logo">
      </div>
      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a :class="{ active: link.current }" :href="link.url">{{link.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      links: [
        {
          text: "characters",
          url: "#",
          current: false,
        },
        {
          text: "comics",
          url: "#",
          current: true,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "tv",
          url: "#",
          current: false,
        },
        {
          text: "games",
          url: "#",
          current: false,
        },
        {
          text: "collectibles",
          url: "#",
          current: false,
        },
        {
          text: "videos",
          url: "#",
          current: false,
        },
        {
          text: "fans",
          url: "#",
          current: false,
        },
        {
          text: "news",
          url: "#",
          current: false,
        },
        {
          text: "shop",
          url: "#",
          current: false,
        },
      ]
    }
  }
}
</script>

<style scoped lang="scss">

  @import '../../assets/style/partials/mixins.scss';
  @import '../../assets/style/partials/variables.scss';

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100px;
    .logo {
      display: flex;
      justify-content: center;
      align-items: center;
      img {
        height: 80px;
      }
    }
    nav {
      height: 100%;
      ul {
        height: 100%;
        @include flex-center;
        li {
          height: 100%;
          list-style: none;
          a {
            height: 100%;
            padding: 0 10px;
            text-decoration: none;
            text-transform: uppercase;
            font-size: 14px;
            font-weight: bold;
            @include flex-center;
            color: #444;
            &.active {
              color: $dc-blue;
              border-bottom: 4px solid $dc-blue;
            }
            &:hover {
              background-color: #ddd;
            }
          }
        }
      }
    }
  }



</style>
