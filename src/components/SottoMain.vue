<template>
  <div class="container">
    <div class="ms_main">
        <div class="ms_icontext">
          <img class="imgbox" src="../assets/img/buy-comics-digital-comics.png" alt="">
          <p>DIGITAL COMICS</p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SottoMain',
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .ms_main{
    height: 150px;
    padding-left: 350px;
    background-color: #0283f8;
    color: white;
    display: flex;
  }

  .ms_icontext{
    display: flex;
    flex-direction: row;
    align-items: center;

    p{
      padding: 0 10px;
    }
  }

  .imgbox{
    height: 60px;
  }

</style>
