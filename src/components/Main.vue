<template>
  <div>
    <div class="jumbotron">
        </div>
      <div class="ms_main2">
        <div class="ms_etichetta">
          CURRENT SERIES
        </div>
        <div class="container">
          <div class="ms_flexcontainer">
            <fumetto 
            v-for="(element, index) in fumetti"
            :key="index"
            :img="element.thumb"
            :series="element.series" />
          </div>
        </div>
        <button class="ms_button">
            CURRENT SERIES
        </button>
    </div>
    <SottoMain/>
  </div>
  
</template>

<script>
import SottoMain from './SottoMain.vue'
import fumettidata from '../data/fumetti.js'
import Fumetto from './fumetto.vue'

export default {
  name: 'Main',
  components: {
    SottoMain,
    Fumetto 
  },
  data(){
        return {
            fumetti: fumettidata
        }
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/partials/variables.scss';
  .ms_main2{
    background-color: black;
    color: white;
    padding: 50px;
    position: relative;

    .ms_etichetta{
      display: inline-block;
      padding: 10px;
      background-color: $DCblue-color;
      font-weight: 900;
      margin-top: -70px;
      margin-left: 250px;
      position: absolute;
    }

  }
.jumbotron{
      height: 400px;
      width: 100%;
      background-image: url("../assets/img/jumbotron.jpg");
      background-size: cover;


    }
  .ms_flexcontainer{
    display: flex;
    flex-wrap: wrap;
  }

  .ms_button{
      background-color:$DCblue-color;
      border: 0;
      padding: 10px 60px;
      color: white;
      font-weight: 600;
      display: block;
      margin: 0 auto;
      margin-top: 60px;
    }

</style>
