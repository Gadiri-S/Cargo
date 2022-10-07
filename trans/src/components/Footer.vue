<template>
  <div class="footer">

<div class="menu-footer">
    <h1>MENU</h1>
   <a><li>Home</li></a> 
 <a href=""><li>Services</li></a>
<a href=""><li>Rates</li></a> 
 <a href=""><li>About us</li></a> 
<a href=""><li>Contact</li></a>   
</div>
    <div class="hours">
        <h1>HOURS</h1>
        <li>Monday to Saturday<br>8:30am - 7pm</li>
    </div>
    <div class="ressources">
        <h1>RESSOURCES</h1>
        <a><li>Request a free quote</li></a> 
 <a href=""><li>Rates</li></a>
<a href=""><li>Our Services</li></a> 
 <a href=""><li>Request a callback</li></a> 

    </div>
    <div class="socials">
        <div class="logo"><img src="../assets/images/logo4.png" alt=""></div>
        <p>Cargo Largo is a Cargo Freight company based in New York City and operating all around the world.</p>
        <div class="icons-social">
            <div class="icon-social"><i class="fab fa-facebook"></i></div>
            <div class="icon-social"><i class="fab fa-linkedin"></i></div>
            <div class="icon-social"><i class="fab fa-twitter-square"></i></div>
            <div class="icon-social"><i class="fab fa-instagram-square"></i></div>

        </div>
    </div>

    

  </div>
</template>

<script>
export default {
name:"Footer"
}
</script>

<style scoped>

.footer {
 display: flex;
 justify-content: space-between;
background: #131341;
padding:3%;

}

.footer h1{
    font-size: 20px;
    padding: 15px 0 15px 0;
    color:white;

}

a:visited{
    color:white;
}

.hours {
    text-align: left;
    width:25%;
}

.menu-footer{
        width:25%;
        text-align: left;

}
.menu-footer li{
    list-style: none;
    font-size: 20px;
    text-align: left;
    padding: 5px 0 5px 0;
}

.ressources{
        text-align: left;
            width:25%;


}
.ressources li{
    list-style: none;
    font-size: 20px;
    text-align: left;
    padding: 5px 0 5px 0;
}
.hours li{
    list-style: none;
    font-size: 20px;
    text-align: left;
    padding: 5px 0 5px 0;
}
.menu-footer a:visited{
color: white;
}

.socials{
    display: flex;
    flex-direction: column;
    width:25%;
        text-align: left;


}
.socials p{
    padding: 10px 0 10px 0;
    text-align: left;
}

.icons-social{
    display: flex;

}
.icons-social i{
    font-size: 30px;
    padding: 10px 30px 15px 0;
    color: white;
    cursor: pointer;

}

@media (max-width:1022px) {

    .footer {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    
    .footer h1{
        font-size:20px
    }
    .hours,.menu-footer,.ressources,.socials{
        width: 100%;
        text-align:center;
        margin-bottom:20px;
    }
        .hours li,.menu-footer li,.ressources li,.socials li{
        width: 100%;
        text-align:center
    }
    .socials p{
        margin-top: 25px;
        text-align: center;
    }

    .icons-social {
        margin: auto;
    }
    
    .icons{
        width: 100%;
        font-size: 14px;
        font-weight: bold;
    }
}
</style>