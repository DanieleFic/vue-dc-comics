<template>
  <div>
    <div class="jumbotron">
        </div>
      <div class="ms_main2">
        <div class="ms_etichetta">
          CURRENT SERIES
        </div>
        <div class="container">
          <fumetti 
            v-for="(element, index) in fumetti"
            :key="index"
            :thumb="element" />
          <h1>
            -->Content goes here-->
          </h1>
        </div>
        <SottoMain/>
    </div>
  </div>
  
</template>

<script>
import fumetti from './fumetti.vue'
import SottoMain from './SottoMain.vue'
import fumettidata from '../data/fumetti'

export default {
  name: 'App',
  components: {
    SottoMain,
    fumetti 
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
    height: 300px;
    background-color: black;
    color: white;

    .ms_etichetta{
      display: inline-block;
      padding: 10px;
      background-color: $DCblue-color;
      font-weight: 900;
      margin-top: -150px;
      margin-left: 300px;
    }

  }
.jumbotron{
      height: 400px;
      width: 100%;
      background-image: url("../assets/img/jumbotron.jpg");
      background-size: cover;


    }
  .container{
    height: 150px;
    display: flex;
    align-items: center;
  }

</style>
