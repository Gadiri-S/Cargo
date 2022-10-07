<template>
  <div class="advantages">

<h1></h1>
    <div class="container-advantages">

        <div class="advantage-pic"> <img src="../assets/images/PNGs/eye.png" alt="" class="img-advantage">
        
        <h2>BEST PRICES <br> ON THE MARKET</h2>
        <p>Consistently get the best prices for every shipment you need to send</p>
        
        </div>
       
       
       
       <div class="advantage-pic"> <img src="../assets/images/PNGs/email-open.png" alt="" class="img-advantage">
       
       <h2>PROFESIONNAL<br> COMMUNICATION</h2>
       <p>Communicate 24/7 we a team of profesionnals eager to help you whatever your needs are.</p>
       </div>



        <div class="advantage-pic"> <img src="../assets/images/PNGs/globe-hand.png" alt="" class="img-advantage">
        
            <h2>SHIPMENTS ALL AROUND <br>THE WORLD</h2>
            <p>We ship your products all around the world without interruption and at the best prices.</p>

        </div>

    </div>


  </div>
</template>

<script>
export default {
name:'Advantages'
}
</script>

<style>

.advantages{
    background: rgb(0, 29, 56);
    opacity: 0.94; 
        padding: auto;
}

.container-advantages {
    display: flex;
    justify-content: space-around;
}

.advantage-pic{
    padding: 15px;
    width: 30%;
}

.advantage-pic h2{
   padding: 10px;
   text-align: center;
}
.advantage-pic p{
    text-align: center;
}

.img-advantage{
    height: 70px;
    margin:auto;
}


@media (max-width:870px) {

    .container-advantages {
    display: flex;
    flex-direction: column;
}
    .advantage-pic{
    width: 90%;
    margin: auto;
}

}
</style>