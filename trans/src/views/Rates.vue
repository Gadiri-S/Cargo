<template>
  <div class="rates">
    <Header/>

    <div class="rates-hero">

  <h1>RATES <br> AND<br> PRICE ESTIMATION</h1>

  
</div>

<Table/>
    <Price/>

    <Footer/>
  </div>
</template>

<script>
import Header from '../components/Header.vue';
import Advantages from '../components/Advantages.vue';
import Services from '../components/Services.vue';
import Price from '../components/Price.vue';
import Contact from '../components/Contact.vue'
import Footer from '../components/Footer.vue';
import Table from '../components/Table.vue'

export default {
  name: 'Home',
  components: {
    Header,Advantages,Services,Price,Contact,Footer,Table
  },
  data(){
    return {

    }
  }
  }
</script>

<style>

.rates{
    min-height: 100vh;
}
.rates-hero{
     background:linear-gradient(rgba(0,0,0,0.75),rgba(0,0,0,0.75)),url('../assets/images/cargo.jpg') ;
    background-position: center;
    background-size: cover;
     background-repeat: no-repeat;
    min-height: 100vh;
    padding: 0;
    margin:0;
}

.rates-hero h1{
  padding-top: 20vh;
  font-size: 80px;
  color: white;

}

@media (max-width:900px) {
  .rates-hero h1{
  font-size: 50px;

}
}
</style>