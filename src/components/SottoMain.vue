<template>
  <div class="ms_main">
    <div class="container">
      <div v-for="(element,indice) in links " :key="indice" class="ms_icontext">
          <img class="imgbox" :src="element.img"  alt="">
          <p>{{element.text}}</p>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SottoMain',
  props: {
    
  },
  data() {
    return{
      links:[
        {
          text: "DIGITAL COMICS",
          img:require("../assets/img/buy-comics-digital-comics.png"),
          current: false,
        },
        {
          text: "DC MERCHANDISE",
          img: require("../assets/img/buy-comics-merchandise.png"),
          current: false,
        },
        {
          text: "SUBSCRIPTION",
          img: require("../assets/img/buy-comics-shop-locator.png"),
          current: false,
        },
        {
          text: "COMIC SHOP LOCATOR",
          img: require("../assets/img/buy-comics-subscriptions.png"),
          current: false,
        },
        {
          text: "DC POWER VISA",
          img: require("../assets/img/buy-dc-power-visa.svg"),
          current: false,
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  .ms_main{
    height: 150px;
    background-color: #0283f8;
    color: white;
  }

  .ms_icontext{
    display: flex;
    flex-direction: row;
    align-items: center;
    padding: 30px 30px;

    p{
      padding: 0 10px;
    }
  }

  .imgbox{
    height: 40px;

    img{
      height: 60px;
    }
  }

  .container{
    display: flex;
    flex-direction: row;
    align-items: center;
    height: 150px;
  }

</style>
