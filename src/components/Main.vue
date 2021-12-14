<template>
  <main>
      <div class="container">
        <h1>
            Content
        </h1>          
      </div>
  </main>
</template>

<script>
export default {
  name: 'Main',
}
</script>

<style scoped lang="scss">
  @import '../assets/style/partials/variables.scss';

    main {
      height: 150px;
      background-color: $dc-gray;
    }
    h1 {
        color: white;
        line-height: 150px;
    }
    
</style>