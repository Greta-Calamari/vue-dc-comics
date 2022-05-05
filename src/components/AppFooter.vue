<template>
<div class="footer">

<div class="footer-container">
  <div class="lists-container">
        <div class="ul-cont">
   <ul>
   <h4 class="titleFooter">DC COMICS</h4>
       <li v-for="(item,index) in links" :key="index" class="sub">{{item.testo}}</li>
   </ul>

 
   <ul>
   <h4 class="titleFooter">DC</h4>
       <li v-for="(item,index) in DC" :key="index" class="sub">{{item.testo}}</li>
   </ul>

   
   <ul>
   <h4 class="titleFooter">SITES</h4>
       <li v-for="(item,index) in sites" :key="index" class="sub">{{item.testo}}</li>
   </ul>

 </div>

 <div class="ul-cont-2">
     <ul>
   <h4 class="titleFooter">SHOP</h4>
       <li v-for="(item,index) in shop" :key="index" class="sub">{{item.testo}}</li>
   </ul>
     


 </div>

 </div>
</div>

<div class="footer2sec">
    <div class="container-subFooter">
        <button class="button">
            <p>SIGN-UP NOW !</p>


        </button>

        <div>
            <ul class="ul-footer">

                <li class="img-as">
                   <h3 class="imp">FOLLOW US</h3>
                </li>
                <li class="img-as">
                    <img src="../assets/img/footer-facebook.png" alt="">
                </li>
                <li class="img-as">
                    <img src="../assets/img/footer-twitter.png" alt="">

                </li>
                <li class="img-as">
                    <img src="../assets/img/footer-youtube.png" alt="">

                </li>
                <li class="img-as">
                    <img src="../assets/img/footer-pinterest.png" alt="">

                </li>
                <li class="img-as">
                    <img src="../assets/img/footer-periscope.png" alt="">

                </li>


            </ul>
        </div>



    </div>

</div>
</div>
 

 

    


</template>





<script>
export default {
  name: 'AppFooter',
  data(){
    return{
          links:[
              {
                  testo:'Characters',
                  link:'',
                  active:false,
              },
              {
                  testo:'Comics',
                  link:'',
                  active:true,
              },
              {
                  testo:'Movies',
                  link:'',
                  active:false,
              },
               {
                  testo:'TV',
                  link:'',
                  active:false,
              },
              {
                  testo:'Games',
                  link:'',
                  active:false,
              },
              
              {
                  testo:'Videos',
                  link:'',
                  active:false,
              },
              
              {
                  testo:'News',
                  link:'',
                  active:false,
              },
            
          ],DC:[
                {
                  testo:'Terms Of Use',
                  link:'',
                  active:false,
                },
                {
                  testo:'Privacy Policy(New)',
                  link:'',
                  active:false,
                },
                {
                  testo:'Add Choices',
                  link:'',
                  active:false,
                },
                {
                  testo:'Advertising',
                  link:'',
                  active:false,
                },
                {
                  testo:'Jobs',
                  link:'',
                  active:false,
                },
                {
                  testo:'Subscriptions',
                  link:'',
                  active:false,
                },
                {
                  testo:'Talent Workshops',
                  link:'',
                  active:false,
                },
                {
                  testo:'CPSC Certificates',
                  link:'',
                  active:false,
                },
                {
                  testo:'Ratings',
                  link:'',
                  active:false,
                },
                {
                  testo:'Shop Help',
                  link:'',
                  active:false,
                },
                {
                  testo:'Contact Us',
                  link:'',
                  active:false,
                },
            ],sites:[
                {
                  testo:'DC',
                  link:'',
                  active:false,
                },
                {
                  testo:'MAD Magazines',
                  link:'',
                  active:false,
                },
                {
                  testo:'DC Kids',
                  link:'',
                  active:false,
                },
                {
                  testo:'DC Unmiverse',
                  link:'',
                  active:false,
                },
                {
                  testo:'DC Power Visa',
                  link:'',
                  active:false,
                },
                
            ],shop:[
                {
                  testo:'Shop DC',
                  link:'',
                  active:false,
                },
                {
                  testo:'Shop DC Collectibles',
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

.footer{
    width: 100%;
    background-image:url(../assets/img/footer-bg.jpg);
    background-size: cover;
}

.footer-container{
    width: 80%;
    margin: 0 auto;
    padding: 20px;
    
}
    
    


.titleFooter{
    color: $fontImp;
    font-size: 18px;
    padding-bottom:10px ;
}

.sub{
    color: $fontColor;
}



.ul-cont{
    
    display: flex;
    gap: 50px;
    
}

// SECONDA SEZIONE FOOTER
.footer2sec{
    width: 100%;
    height: 100px;
    background-color: $background;
    
}
.container-subFooter{
    display: flex;
    justify-content: space-between;
    width: 80%;
    margin: 20px auto
    
}

.button{
    border: 3px solid $blueDc;
    width: 150px;
    padding: 14px;
    font-size: 15px;
    background: none;
    color: $fontImp;
    margin-top: 20px;
}
.imp{
    
    color: $blueDc;
    
}
.img-as{
    display: inline-block;
    padding: 10px;
}

.ul-footer{
    margin-top: 20px;
}
    








</style>
    


    

