<template>
  <div class="contact">

   <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3025.444414068222!2d-74.00935396456056!3d40.68620900214599!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c25a5d85d5cb7f%3A0x40b6bf2f255d6f51!2sRed%20Hook%20Terminal!5e0!3m2!1sfr!2sfr!4v1659281874275!5m2!1sfr!2sfr" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>



<div class="quote">

    <div class="quote-text">
    <h2>Get a free quote</h2>
    <p>Fill the form and receive directly by email a free quote</p>
    <p>You can also, if you wish, receive a callback</p>

    <form action="">
        <input type="text" placeholder="Your name*">
        <input type="tel" placeholder="Phone number*">
        <button>Send to receive a callback</button>
    </form>
    </div>

    <div class="quote-form">
        <form action="">
            <input type="text" placeholder="First name*" required>
            <input type="text" placeholder="Last name*" required>
            <input type="tel" placeholder="Phone number*" required>
            <input type="email" placeholder="Email*" required>
            <textarea name="message" id="message" cols="20" rows="5" placeholder="Message"></textarea>

            <button class="button-form">Send to receive a free quote</button>


        </form>
    </div>

</div>
            <button class="call">Call us +554 584 269</button>


  </div>
</template>

<script>
export default {

    name:'Contact'

}
</script>

<style scoped>

.contact {
 
    min-height: 100vh;
    padding: 2% 0 0 0 ;
    color:white;
    background: rgb(0, 29, 56);
    opacity: 0.94; 
}

.quote{
    display: flex;
    min-height: 70vh;
    margin-top: 25px;
}
.quote-text{
    width: 40%;
}

.quote-text form input{
    width:80%;
     height: 30px;
    padding: 5px 0 5px 15px;
    background: transparent;
        border: 1px solid white;
border-radius:4px;
    margin: 15px 10px 15px 0px;
    font-size: 17px;
    color: white;
    font-family: 'Poppins', sans-serif;
    
}
.quote-text form button{
     width:80%;
    background: transparent;
    color: white;
        font-family: 'Poppins', sans-serif;
        border: 1px solid white;
        padding: 5px;
        font-size: 20px;
        cursor: pointer;
}

.quote-text form button:hover{
transition: .4s;
    background: crimson;
    border: none;

}


.quote-text h2{
font-size: 25px;
margin-bottom:15px;
}
.quote-form{
    display: flex;
    width: 60%;
}
.quote-form input{
    width: 40%;
    height: 30px;
    padding: 5px 0 5px 15px;
    background: transparent;
        border: 1px solid white;
border-radius:4px;
    margin: 0 10px 15px 0px;
    font-size: 17px;
    color: white;
    font-family: 'Poppins', sans-serif;
}

#message{
    width:85%;
    background:transparent;
    margin: 15px 15px 15px 0;
        font-size: 17px;
    color: white;
    font-family: 'Poppins', sans-serif;
        padding: 5px 0 5px 15px;

}

.button-form{
    width:80%;
    background: transparent;
    color: white;
        font-family: 'Poppins', sans-serif;
        border: 1px solid white;
        padding: 5px;
        font-size: 20px;
        cursor: pointer;

}

.button-form:hover{
    background: crimson;
    color: white;
        border: none;
}

::placeholder {
    color: white;
}

iframe{
    width: 100%;
}

.quote-text p{
    font-size: 20px;
}

.call {
    width:20%;
    background:crimson;
     font-family: 'Poppins', sans-serif;
        border: none;
        padding: 10px;
        font-size: 20px;
        cursor: pointer;
        color:white;
        border-radius: 15px;
        margin:auto auto 50px auto
}

@media (max-width:950px) {
    
    .quote{
        display: flex;
        flex-direction: column;
    }

.quote-text{
    width: 100%;
    margin-bottom: 50px;
}

.quote-form{
    width: 100%;
}

.call {
    width:80%;
    background:crimson;
     font-family: 'Poppins', sans-serif;
        border: none;
        padding: 10px;
        font-size: 20px;
        cursor: pointer;
        color:white;
        border-radius: 15px;
        margin:50px auto 50px auto
}
}
</style>