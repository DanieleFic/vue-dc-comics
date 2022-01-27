<template>
  <div class="Header">
    <div class="preheader">

    </div>
    <div class="container">
      <div class="ms_menu">
      <img src="../assets/img/dc-logo.png" alt="">
      <ul>
        <li v-for="(element,indice) in links " :key="indice"><a href="#">{{element.text}}</a></li>
        
      </ul>
    </div>
    </div>
    
    
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return{
      links:[
        {
          text: "Carachters",
          url: "#",
          current: false,
        },
        {
          text: "Comics",
          url: "#",
          current: false,
        },
        {
          text: "Movies",
          url: "#",
          current: false,
        },
        {
          text: "TV",
          url: "#",
          current: false,
        },
        {
          text: "Games",
          url: "#",
          current: false,
        },
        {
          text: "Collectibles",
          url: "#",
          current: false,
        },
        {
          text: "Videos",
          url: "#",
          current: false,
        },
        {
          text: "Fans",
          url: "#",
          current: false,
        },
        {
          text: "News",
          url: "#",
          current: false,
        },
        {
          text: "Shop",
          url: "#",
          current: false,
        },
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
//@import '../src/assets/style/partials/variables.scss';

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #000000;
  text-decoration: none;
  font-weight: 400;
}
.preheader{
  height: 100px;
  background-color: black;
}

.ms_menu{
  background-color: white;
  display: flex;
  justify-content: space-around;
  align-items: center;
  margin: 20px 15px;
}

</style>
