<template>
<div>

       <Header/>


 <div class="home">

        <div class="front-title">
      <h1>CARGO LARGO</h1>
      </div>


  <div class="box">
    <div ><button class="box-price" @click="nav(contact[0].id)">GET A QUOTE</button></div>
        <div ><button class="box-contact" @click="nav(price[0].id)">PRICE ESTIMATION</button></div>

  </div>

  <div class="box-explore">
<button @click="nav(services[0].id)">OUR SERVICES</button>  </div>



</div>
  
  <Services id='services'/>
  
      <Price id='price'/>

    <Advantages/>


  <Contact id='contact'/>

  <Footer/>

  </div>
</template>

<script>
// @ is an alias to /src

import Header from '../components/Header.vue';
import Advantages from '../components/Advantages.vue';
import Services from '../components/Services.vue';
import Price from '../components/Price.vue';
import Contact from '../components/Contact.vue'
import Footer from '../components/Footer.vue'

export default {
  name: 'Home',
  components: {
    Header,Advantages,Services,Price,Contact,Footer
  },
  data(){
    return {

      contact: [
   {
id: 'contact'}],
price: [
   {
id: 'price'}],
 services: [
   {
id: 'services'}],

    }
  },
  methods:{
    nav(id) {

const position = document.getElementById(id).offsetTop;
  // smooth scroll
 window.scrollTo({ top: position, behavior: "smooth" });  
},
  }
}
</script>
<style>


*{
  padding: 0;
  margin: 0;
}

.home{
   background:linear-gradient(rgba(0,0,0,0.65),rgba(0,0,0,0.65)),url('../assets/images/wallpaper.jpg') ;
   color:white;
    background-position: center;
    background-size: cover;
     background-repeat: no-repeat;
    min-height: 100vh;
    padding: 0;
    margin:0;
}

.container-title {
  display: flex;
  justify-content: center;
  align-items:baseline;
}
.front-title h1{
  color: white;
  font-weight: 700;
  font-size: 100px;
font-family: 'Ibarra Real Nova', serif  ;
padding-top: 10%;
}



.subtitle {
  color: white;
  font-size: 25px;
  font-family: 'Ibarra Real Nova', serif  ;

  }


  .box{
    display: flex;
    justify-content: center;
    margin: 10vh  0 50px 0;
  }

  .box-price{
    width: 180px;
    height: 50px;
    margin: 0 25px 0 0;
    font-size: 17px;
    background: transparent;
    color: white;
    font-weight: bold;
    border: 1px solid white;
    cursor: pointer;
  }
  .box-contact{
        width: 180px;
        height: 50px;
        margin: 0 0 0 25px;
            font-size: 17px;
         background: transparent;
    color: white;
    font-weight: bold;
    border: 1px solid white;
        cursor: pointer;
  }

  .box-price:hover{
    transition: .4s;
    background: crimson;
  }
  .box-contact:hover{
       transition: .4s;
    background: crimson;
  }

  .box-explore button{
    background:crimson;
    width: auto;
    border: none;
    border-radius: 5px;
    margin-top: 0;
    font-size: 20px;
    color: white;
    font-weight: bold;
    padding: 20px;
    cursor:pointer;
  }
  .box-explore button:hover{
       transition: .4s; 
    background: transparent;
        border:1px solid white;


  }


@media (max-width:800px) {

  .front-title h1{
  color: white;
  font-weight: 700;
  font-size: 80px;
font-family: 'Ibarra Real Nova', serif  ;
padding-top: 30%;
}
  

  .box-price{
width: auto;
padding: 10px;
  }
   .box-contact{
    width: auto;
    padding: 10px;

    
  }

  .box-explore button{
    margin-bottom: 50px;
  }
}
</style>