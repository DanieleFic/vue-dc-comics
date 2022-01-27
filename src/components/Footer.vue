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
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">Forum</a></li>
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

.ms_footer{
  background-image: url("../assets/img/footer-bg.jpg");
}

.msli{
  display: flex;
  flex-direction: row;
  padding: 30px 10px;
  color: white;

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
    background-color: #303030;
    margin: 0 auto;
    padding: 25px 15px;

    .ms_button{
      background-color: #303030;
      border: 2px solid #0283f8;
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
    color: #0283f8;
    font-weight: 900;
  img{
    padding: 0 13px ;
  }
}

</style>
