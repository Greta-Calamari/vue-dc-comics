<template>
<div class="logo">
  
  <img src="../assets/img/dc-logo.png" alt="">

<nav>
    
  <ul>
    <li v-for="(item,index) in links" :key="index" class="nav-bar" :class="{'selected' : item.active}">{{item.testo}}</li>
  </ul>
  
</nav>
</div>




</template>

<script>
export default {
  name: 'AppHeader',
  data(){
    return{
          links:[
              {
                  testo:'CHARACTERS',
                  link:'',
                  active:false,
              },
              {
                  testo:'COMICS',
                  link:'',
                  active:true,
              },
              {
                  testo:'MOVIES',
                  link:'',
                  active:false,
              },
               {
                  testo:'TV',
                  link:'',
                  active:false,
              },
              {
                  testo:'GAMES',
                  link:'',
                  active:false,
              },
              {
                  testo:'COLLECTIBLES',
                  link:'',
                  active:false,
              },
              {
                  testo:'VIDEOS',
                  link:'',
                  active:false,
              },
              {
                  testo:'FANS',
                  link:'',
                  active:false,
              },
              {
                  testo:'NEWS',
                  link:'',
                  active:false,
              },
              {
                  testo:'SHOP',
                  link:'',
                  active:false,
              },
          ]
      }
  }
  
}
</script>


<style scoped lang="scss">
@import './style/generals';
@import './style/variables';


.nav-bar{
  display: inline-block;
  padding: 5px;
}
.logo{
  width: 80%;
  display: flex;
  justify-content: space-around;
  margin-top: 30px;
  margin-bottom: 20px;
}

nav{
  padding-top:40px ;
}

.selected{
  color: $blueDc;
  margin-bottom: 10px;
  border-bottom:5px solid $blueDc;
  
}



</style>
