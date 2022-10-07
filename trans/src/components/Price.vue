<template>
  <form action="" v-on:submit.prevent="onSubmit" class="calculator">

<div class="location">

    <div>
  <h1>Where <br> is the shipment?</h1>
<select name="size" id="size">
    <option value="20ft">Europe</option>
    <option value="40ft">North America</option>
    <option value="45ft">South America</option>
    <option value="45ft">North Africa</option>
    <option value="45ft">Western Africa</option>
    <option value="45ft">Eastern Africa</option>
    <option value="45ft">South Asian</option>
    <option value="45ft">East Asia</option>
    <option value="45ft">Pacific</option>

</select>
</div>


<div>
<h1>Where <br> do you want to ship it?</h1>
<select name="size" id="size">
    <option value="20ft">Europe</option>
    <option value="40ft">North America</option>
    <option value="45ft">South America</option>
    <option value="45ft">North Africa</option>
    <option value="45ft">Western Africa</option>
    <option value="45ft">Eastern Africa</option>
    <option value="45ft">South Asia</option>
    <option value="45ft">East Asia</option>
    <option value="45ft">Pacific</option>

</select>
</div>
</div>

<h1>Select a container size</h1>
<select name="size" id="size">
    <option value="20ft">20ft</option>
    <option value="40ft">40ft</option>
    <option value="45ft">45ft</option>

  
</select>


<div>
 
 <input type="number" id="distance" class="distance" placeholder="Distance in Kilometers" required min="10" max="25000"  v-model="distance">
</div>



    <button @click="calc" class="calculate-button">Calculate</button>

     <div v-if="finalPrice"><p class="price">We estimate the cost of your shipment at {{finalPrice}}. <br> Please for more information request a free quote or contact us directly</p>
                <div class="contact-price">
                    <button>Request a free quote</button>
                    <button>Contact us</button>
                    <button>Call us +554 584 269</button>
                </div>
                </div> 
  </form>

</template>

<script>
export default {

data() {
    return {

       distance: this.distance,
       finalPrice: '',
       error:''
    }
},
methods:{
    calc(){

        const size = document.getElementById('size').value;
        const distance = document.getElementById('distance').value;
        let distanceBase = distance*0.35;
        let basePrice = '';
        let finalPrice ='';
        const error = "Error";


        if(size == '20ft'){
            basePrice = 250
        } else if (size == '40ft') {
            basePrice = 450
        } else if (size == '45ft') {
            basePrice = 650
        }


        if(distance > 25000 || distance <10) {

            const error = "Error";
            console.log(error)
            return error
        }

       
       finalPrice = '$ '+ Math.round((basePrice+distanceBase)*100)/100;

       this.finalPrice = finalPrice

       console.log(finalPrice)



    }
}
}
</script>

<style>

.calculator {
display: flex;
flex-direction: column;
justify-content: space-evenly;
align-items: center;

    color: black;
    background: white;
    

    margin:3%;
    padding: 3%;

    min-height: 50vh;
}

.location{
    display: flex;
}
.location h1{
    margin-right: 15px;
}

h1{
    font-size: 40px;
    color: crimson;
}
    #distance{
  font-size: 25px;
    width: 450px;
    height: 50px;   
    margin: 20px auto 20px auto; }

 #size{
    font-size: 25px;
    width: 450px;
    height: 50px;
    margin: 20px auto 20px auto; 
 }



.price{
    font-size: 25px;
    padding: 25px;
}


input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
  -webkit-appearance: none;
  margin: 0;
}
.calculate-button{
    padding: 10px;
    border: none;
    background: crimson;
    color: white;
    border-radius: 10px;
    cursor:pointer;
        font-family: 'Poppins', sans-serif;
        font-size:20px;

}

::placeholder{
    font-size: 20px;
    font-family: 'Poppins', sans-serif;

    
}

.contact-price button{
        font-size: 20px;
    font-family: 'Poppins', sans-serif;
    background: crimson;
    color:white;
    padding: 10px;
    border-radius: 10px;
    margin: 25px 15px 25px 15px;
    border: none;
    cursor:pointer;

}

@media (max-width:1200px) {

    h1{
    font-size: 30px;
    color: crimson;
}

.location{
    display: flex;
    flex-direction: column;
}
    #distance{
  font-size: 20px;
    width: 88vw;
    height: 50px;   
    margin: auto; }

 #size{
    font-size: 25px;
    width: 100%;
    height: 50px;
    margin: 20px auto 20px auto; 
 }



.price{
    font-size: 25px;
    padding: 25px;
}

.calculate-button {
    margin-top: 20px;
}
    
}
    
</style>