

<template>
  <div class="services">

<h1>CARGO LARGO SERVICES</h1>
<div class="underline-title"></div>
      <div class="card-container">
   
      <div class="card center">
           <img src="../assets/images/wallpaper.jpg"  class="img" alt="">
                   <span class="title">Sea Cargo</span>

      </div>
      <div class="card center">
           <img src="../assets/images/packing.png"  class="img" alt="">
                   <span class="title">Packing & Packaging</span>

      </div>
      <div class="card center">
                 <img src="../assets/images/conteneurs.jpg"  class="img" alt="">
                         <span class="title">Shipment tracking</span>

            </div>
            <div class="card center">
                 <img src="../assets/images/insurance.jpg"  class="img" alt="">
                         <span class="title">Insurance management</span>

            </div>
            <div class="card center">
                 <img src="../assets/images/4.jpg"  class="img" alt="">
                         <span class="title">Warehousing</span>

            </div>
      <div class="card center">
           <img src="../assets/images/logistics.jpg"  class="img" alt="">
        <span class="poll"></span>

                   <span class="title">Logistics Solutions</span>

      </div>
      <div class="card center">
           <img src="../assets/images/clearance.jpg"  class="img" alt="">
    <span class="poll">We will handle all the administrative paperwork for you with our team of experienced profesionnals.</span>

                   <span class="title">Customs Clearance</span>

      </div>

      <div class="card center">
           <img src="../assets/images/communication.jpg"  class="img" alt="">
                              <span class="poll">Thanks to our very reactive team, contact us whenever you need to. We'll always find time for you.</span>

                   <span class="title">24/7 Assistance</span>

      </div>


      </div>

      <div class="level">
       <div class="container-img-level"> <img src="../assets/images/docks.jpg" alt=""></div>
       <h1>GO <br> TO <br> THE NEXT LEVEL</h1>
      </div>
  </div>
</template>

<script>
export default {

    data(){
        return {

        }
    },
    methods:{
        showText(){
        const tool = document.querySelector('.poll').className='pooi'
        }
    }

}
</script>

<style scoped>

.level {
    display: flex;
}



.level img{
    height: 500px;
    width:100%;
    object-fit: cover;
    clip-path: polygon(0 0, 100% 0%, 75% 100%, 0% 100%);

}

.level h1{
    font-size: 80px;
}

.container-img-level{
    width:90%;
}
.services {
    background: white;
            min-height: 100vh;


}
.poll{
    display: none;
 }
 
h1 {

    font-size: 50px;
        padding: 25px;
        color:  crimson;;

}
.underline-title {
     width: 80px;
    height: 7px;
    background:  crimson;;
    margin: 5px auto 40px auto;
}
.card-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.img {
    height: 250px;
    width: 350px;
    object-fit: cover;
}


 .pooi{
   
    display: block;
    position: absolute;
    max-width:350px;
    text-align: center;
    margin: 50px 0 0 0;
    color:white;
}

.title {
   position: absolute;
  background:  crimson;
    font-size: 17px;
    padding: 5px;
    color: white;
}  
.card {
    display: flex;
  flex-flow: row nowrap;
  align-items: flex-start;
  justify-content: flex-start;
  position: relative;
  padding: 10px;
  text-align: center;
  font-size: 1.2rem;
  color: white;
  width: 350px;
  cursor: pointer;
}


.center {
        align-self: flex-end;
;

}



@media (max-width:1000px) {


.level h1{
    font-size: 40px;
    padding: 0;
}

.level img{
    height: 300px;
    width:100%;
    object-fit: cover;
    clip-path: polygon(0 0, 100% 0%, 75% 100%, 0% 100%);

}

}





@media (max-width:700px) {

    .services {
        height: auto;
    }
    .card-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        margin: auto;
        padding: auto;
        overflow-x: hidden;
    }

    .img:hover + .poll{
   
    display: block;
    position: absolute;
    max-width: 100%;
    text-align: center;
    margin: 50px 0 0 0;
    color:white;
}
 .poll:hover{
   
    display: block;
    position: absolute;
    max-width: 100%;
    text-align: center;
    margin: 50px 0 0 0;
    color:white;
}
.card {
    width: 100%;
    padding: 0;
}
.img {
    width: 100vw;
}
 .card center {
     padding: 0;
 }



 
}

@media (max-width:701px) {
}
</style>

