<template>
  <div class="ms_footer">
    <div class="container">
      <div class="msli">
        <div class="firstLI">
        <h3>DC COMICS</h3>
      <ul>
        <li><a href="#">Core Docs</a></li>
        <li><a href="#">Forum</a></li>
        <li><a href="#">Community Chat</a></li>
        <li><a href="#">Twitter</a></li>
        <li><a href="#">News</a></li>
        <li><a href="#">Twitter</a></li>
        <li><a href="#">News</a></li>
      </ul>
    <h3>SHOP</h3>
      <ul>
        <li><a href="#" target="_blank" rel="noopener">Core Docs</a></li>
        <li><a href="#" target="_blank" rel="noopener">Forum</a></li>
      </ul>
        </div>
      <div class="secondLI">
        <h3>DC</h3>
        <ul>
          <li><a href="#" >Core Docs</a></li>
          <li><a href="#">Forum</a></li>
          <li><a href="#">Community Chat</a></li>
          <li><a href="#">Twitter</a></li>
          <li><a href="#">News</a></li>
          <li><a href="#">Forum</a></li>
          <li><a href="#">Community Chat</a></li>
          <li><a href="#">Twitter</a></li>
          <li><a href="#">News</a></li>
          <li><a href="#">Core Docs</a></li>
          <li><a href="#">Forum</a></li>
        </ul>
      </div>
        <div class="thirdLI">
          <h3>SITES</h3>
          <ul>
            <li><a href="#">Core Docs</a></li>
            <li><a href="#">Forum</a></li>
            <li><a href="#">Community Chat</a></li>
            <li><a href="#">Twitter</a></li>
            <li><a href="#">News</a></li>
          </ul>
        </div>
      </div>
      <div class="logoimg">
          <img src="../assets/img/dc-logo-bg.png" alt="">
        </div>
    </div>
    
    <div class="ms_secondfooter">
      <div class="container">
        <button type="button" class="ms_button">SIGN-UP NOW!</button>
        <div class="ms_social">
          <span>FOLLOW US</span>
          <img src="../assets/img/footer-facebook.png" alt="">
          <img src="../assets/img/footer-periscope.png" alt="">
          <img src="../assets/img/footer-pinterest.png" alt="">
          <img src="../assets/img/footer-twitter.png" alt="">
          <img src="../assets/img/footer-youtube.png" alt="">
        </div>
      </div>
  </div>
      </div>
        
</template>

<script>
export default {
  name: 'Footer',
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/partials/variables.scss';
.ms_footer{
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
}

.container{
    display: flex;
    justify-content: space-between;

    .logoimg{
      height: 500px;
      margin: -30px;
    }
  }

.msli{
  display: flex;
  flex-direction: row;
  padding: 30px 10px;
  color: white;

  img{
    height: 450px;
  }

  .firstLI{
    padding-right:30px;
  }
  .secondLI{
    padding-right:30px;
  }
  .thirdLI{
    padding-right:30px;
  }

  h3{
    padding: 15px 0px;
  }

  ul li{
    list-style-type: none;
    font-size: 13px;
    color: gray;
    padding: 3px 0px;
    
    a{
      text-decoration: none;
      color: gray;
    }
  }
}

.ms_secondfooter{
    height: 100px;
    background-color: $footer-color;
    margin: 0 auto;
    padding: 25px 15px;
    position: relative;

    .ms_button{
      background-color: $footer-color;
      border: 2px solid $DCblue-color;
      color: white;
      padding: 15px;
    }

    .container{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
  }
  }

.ms_social{
    display: flex;
    align-items: center;
    color: $DCblue-color;
    font-weight: 900;
  img{
    padding: 0 13px ;
  }
}

</style>
