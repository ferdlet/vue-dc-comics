<template>
    <section id="series">
        <div class="container">
            <div class="title-section">
                Current Series
            </div>
            <div class="container-series">
                <CardSerie  v-for="(serie, index) in series" :key="index" :serie="serie"/>
            </div>
            <a href="#">Load More</a>
        </div>
    </section>  
</template>

<script>
import CardSerie from '../commons/CardSerie.vue'
import series from '../../data/currentSeries.js'

export default {
  name: 'CurrentSeries',
  components: {
    CardSerie,
  },
  data() {
    return {
        series: series
    }
  }

}
</script>

<style scoped lang="scss">
    @import '../../assets/style/partials/mixins.scss';
    @import '../../assets/style/partials/variables.scss';
  
    #series {
        background-color: $dc-gray;
        .container {
            position: relative;
            padding: 20px;
            .title-section {
                color: white;
                text-transform: uppercase;
                padding: 10px 20px;
                background-color: $dc-blue;
                display: inline-block;
                position: absolute;
                top: -20px;
                left: 10px;
                font-weight: bold;
            }
            .container-series {
                margin-bottom: 10px;
                padding: 40px 0;
                display: flex;
                justify-content: center;
                flex-wrap: wrap;
                > * {
                    width: calc(100% / 6 - 20px);
                    margin: 0 10px;
                    margin-bottom: 40px;
                }
            }
            a {
                text-decoration: none;
                color: white;
                text-transform: uppercase;
                padding: 10px 50px;
                background-color: $dc-blue;
                font-weight: bold;
                display: inline-block;
                font-size: 14px;
                position: absolute;
                left: 50%;
                bottom: 20px;
                transform: translateX(-50%);
            }
        }
    }
</style>