<template>
  <main>
      <Jumbotron/>
      <CurrentSeries/>
  </main>
</template>

<script>
import Jumbotron from './../sections/Jumbotron.vue'
import CurrentSeries from './../sections/CurrentSeries.vue'


export default {
  name: 'Main',
  components: {
    Jumbotron,
    CurrentSeries,
  }
}
</script>

<style scoped lang="scss">
  @import '../../assets/style/partials/variables.scss';
    
</style>