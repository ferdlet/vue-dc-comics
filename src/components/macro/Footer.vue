<template>
  <footer>
    <FooterTop/>
    <FooterBody/>
    <FooterBottom/>

   
  </footer>
</template>

<script>
import FooterTop from './../sections/FooterTop.vue'
import FooterBody from './../sections/FooterBody.vue'
import FooterBottom from './../sections/FooterBottom.vue'


export default {
  name: 'Footer',
  components: {
    FooterTop,
    FooterBody,
    FooterBottom,
  },
  
}
</script>

<style scoped lang="scss">

</style>
