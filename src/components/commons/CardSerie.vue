<template>
  <div class="serie">
    <a href="#">
        <div class="image">
            <img :src="serie.thumb" :alt="serie.series">
        </div>
        <p>{{serie.series}}</p>
    </a>
  </div>
</template>

<script>
export default {
    name: 'CardSerie',
    props: {
        serie: Object
    }
}
</script>

<style scoped lang="scss">
    .serie {
        a {
            text-decoration: none;
            display: flex;
            flex-direction: column;
            color: white;
            .image {
                margin-bottom: 15px;
                height: 180px;
                overflow-y: hidden;
                img {
                    width: 100%;
                }
            }
            p {
                font-size: 14px;
                text-transform: uppercase;
            }
            
        }
    }
</style>