<template>
  <footer>
    <div class="container">
      
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

  @import '../assets/style/partials/mixins.scss';

  



</style>
