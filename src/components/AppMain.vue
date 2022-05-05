<template>
<div class="container">
    <div class="card-container">
        

    </div>
    
    
    
    <div class="container secondC">
        <ul class="nav-useful" >
            
            <li class="li-nav" v-for="(item,index) in usefulLinks" :key="index" ><img :src="item.img" alt="" class="img-w">{{item.testo}}</li>
                
        </ul>

    </div>

            


</div>

</template>





<script>



export default {
  name: 'AppMain',

        
  
  data(){
      return{
          usefulLinks:[
              {
                  testo:'DIGITAL COMICS',
                  img:require('../assets/img/buy-comics-digital-comics.png'),
                  link:'',
                  active:false,
              },
              {
                  testo:'DC MERCHARDISE',
                  img:require('../assets/img/buy-comics-merchandise.png'),
                  link:'',
                  active:true,

              },
              {
                  testo:'SUBSCRIPTION',
                  img:require('../assets/img/buy-comics-subscriptions.png'),
                  link:'',
                  active:false,

              },
               {
                  testo:'COMIC SHOP LOCATOR',
                  img:require('../assets/img/buy-comics-shop-locator.png'),
                  link:'',
                  active:false,
              },
              {
                  testo:'DC POWER VISA',
                  img:require('../assets/img/buy-dc-power-visa.svg'),
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

.container{
    
    background-color:$background ;
}
   
.card-container{
    width: 80%;
    margin: 0 auto;
    padding: 40px;
    color:$fontImp;
}

// SECONDA SECTION MAIN
.secondC{
    background-color: $blueDc;
    color: $fontImp;
}

.nav-useful{
    display: flex;
    justify-content: space-around;
    padding: 10px;
    width: 80%;
    margin: 0 auto;
    
}

.img-w{
    width: 50px;
    height: 65px;
    vertical-align: middle;
}
.li-nav{
    display: inline-block;
    padding: 10px;
}
    
    
   
    




</style>
