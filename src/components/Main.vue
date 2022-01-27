<template>
  <div class="ms_main2">
    <div class="container">
        <h1>
          -->Content goes here-->
        </h1>
    </div>
    <SottoMain/>
  </div>
</template>

<script>
import SottoMain from './SottoMain.vue'
export default {
  name: 'App',
  components: {
    SottoMain,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .ms_main2{
    height: 300px;
    margin-top: 15px;
    background-color: black;
    color: white;
    
  }

  .container{
    height: 150px;
    display: flex;
    align-items: center;
  }

</style>
