<template>
<div class="about">

       <Header/>


<div class="about-hero">

  <h1>GET TO KNOW US</h1>

  <img src="../assets/images/arrowdown.png" alt="" class="arrow">
  
</div>


<div class="message-president">
  <div class="text-message">
    <h1>WHAT WE BELIEVE IN</h1>
  <p>Cargo Largo started from a strong desire to answer the need of profesionnalism, honesty and quality work in the transport industry.</p>
  <p>Here, we are dedicated to always put the customer first, no matter what.</p>
  <p>Our team is rich in experience and profiles. Everybody has a place at Cargo Largo!</p></div>
    <p class="signature">Marshall J. Watson, Founder & President of Cargo Largo</p>

</div>

<div class="team">
  <h1>CARGO LARGO AT WORK</h1>
  <div class="team-pictures">
  <div class="team-picture"> <img src="../assets/images/1.jpg" alt="" class="picture-team"></div> 
    <div class="team-picture"> <img src="../assets/images/2.jpg" alt="" class="picture-team"></div> 
  <div class="team-picture"> <img src="../assets/images/3.jpg" alt="" class="picture-team"></div> 
  <div class="team-picture"> <img src="../assets/images/worker.jpg" alt="" class="picture-team"></div> 
  <div class="team-picture"> <img src="../assets/images/4.jpg" alt="" class="picture-team"></div> 
  <div class="team-picture"> <img src="../assets/images/5.jpg" alt="" class="picture-team"></div> 

  </div>
</div>


<Contact/>


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

    }
  }
  }

</script>
<style>

.about{
  min-height: 100vh;
}




.message-president {
    padding: 15px;
    margin: auto;
   background: #131341;
;
    

}
.message-president h1{
  font-size: 60px;
  color:crimson;
  padding: 30px 0 30px 0;
}
.text-message{
  color: white;
  font-size: 25px;
  line-height: 1.5;
}
.signature{
  font-size:35px;
  font-family: 'Herr Von Muellerhoff', cursive;

  color:white;

}
.about-hero{
     background:linear-gradient(rgba(0,0,0,0.75),rgba(0,0,0,0.75)),url('../assets/images/1.jpg') ;
    background-position: center;
    background-size: cover;
     background-repeat: no-repeat;
    min-height: 100vh;
    padding: 0;
    margin:0;
}

.about-hero h1{
  padding-top: 40vh;
  font-size: 80px;
  color: white;

}

.arrow{
  height: 70px;
  cursor:pointer;
  border-radius: 50%;
  padding:10px;
}
.arrow:hover{
  transition: .4s;
    background: crimson;
}

.team-pictures{
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.team-picture {
  width: 32%;
  padding: 5px;
}

.team{
  padding-top: 25px;
}
.team h1{
  color:crimson;
  font-size: 60px;
  font-weight: bold;
}

.picture-team{
height: 50vh;
width:100%;
object-fit: cover;
}

@media (max-width:980px) {
  .president {
    display: flex;
    flex-direction: column;
  }

  .team-pictures{
        display: flex;
    flex-direction: column;
  }
  .team-picture{
    width:100%;
    margin: auto;
    padding:0;
  }

  .message-president{
    width: auto;
    padding: 5px;
  }
  .picture-ceo{
     height:50vh;
     width: 100%;
}

.about-hero h1{
  padding-top: 40vh;
  font-size: 50px;
  color: white;

}


.signature{
  font-size:25px;
  margin-top: 15px;
  font-family: 'Herr Von Muellerhoff', cursive;


}

.message-president h1{
  font-weight:700;
  font-size: 35px;
}

}

</style>