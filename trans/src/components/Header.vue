<template>

<div class="main-nav" id="main-nav">
<!--Debut Version Desktop and tablets-->

          <div class="header">
            <div class="logo" id="logo"> <img src="../assets/images/logo4.png" alt=""> </div>

            <div class="menu">
          <router-link to="/"> <a href=""><li>Home</li></a> </router-link>
          <router-link to="/rates"> <a href=""><li>Rates</li></a> </router-link>
          <router-link to="/about"> <a href=""><li>About us</li></a> </router-link>
            <a @click="nav(contact[0].id)"><li>Contact</li></a>

            </div>
            </div>

            <!--Fin  Version Desktop and tablets-->



              <!--Debut Menu version responsive for small screens (phones)-->

                          <div class="header-phone"> 


                                <div class="container-icons-header">
                            <div ><img src="../assets/images/logo4.png" alt="" class="logo"></div>


                            <div v-if="show == true"><img src="../assets/images/burgerwhite.png" alt="" class="burger" @click="burger"></div>
                            <div v-else><img src="../assets/images/close.png" alt="" class="burger" @click="burger"></div>

                            
                            </div>

                            <div v-if="show == false">                         

          <router-link to="/"> <a href=""><li>Home</li></a> </router-link>
              <a href=""><li>Services</li></a>
          <router-link to="/rates"> <a href=""><li>Rates</li></a> </router-link> 
          <router-link to="/about"> <a href=""><li>About us</li></a> </router-link>
            <a href=""><li>Contact</li></a>
             </div>
            </div>

                          <!--Fin Version small screens-->


</div>
</template>

<script>

export default {
      name: 'Header',
      
   
        data(){
            return {

            show:false,

            contact: [
   {
id: 'contact'}],
 services: [
   {
id: 'services'}],
 
            }
        },
        beforeMount(){
this.burger()

        },
        mounted() {
                                this.changeColor()

        },
      
        methods:{
            burger(){

                this.show = !this.show

                
            },
            nav(id) {

const position = document.getElementById(id).offsetTop;
  // smooth scroll
 window.scrollTo({ top: position, behavior: "smooth" });  
},
            changeColor(){

                const header = document.getElementById('main-nav');

                console.log(header)

document.addEventListener('scroll', function() {
  
  // Get the scroll position
  let scrollPos = window.pageYOffset;
  
  if ( scrollPos < 95 ) {
    header.style.backgroundColor = "transparent";
  } else {
    header.style.backgroundColor = "#171772aa";
  }
  
  
})/**/;
            }
            
        }}

</script>

<style>

#main-nav{
    position: fixed;
    width: 100%;
    margin-bottom: 15%;
 background: transparent;
     z-index: 999;

}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px;
}
.header-phone{
    display: none;
}
.menu {
    display: flex;
    font-family: 'Lato', sans-serif;

}
.menu li {
    list-style: none;
    padding: 0 15px 0 15px ;
    font-size: 22px;
    color: white;
}

.menu li:hover {
    cursor: pointer;
    transition: .4s;

}
.logo img{
    height: 70px;
}

.menu-phone{
    display: none;
}

@media (max-width:800px) {

    .header {
        display: none;
    }

    .header-phone{
        display: block;
    }

    .container-icons-header{
        display: flex;
        justify-content: space-between;
        width: 100%;

    }
    .header-phone .logo{
        padding: 15px;
        height: 40px;
    }
    .burger {
        height: 30px;
        padding: 15px;
    }
    .menu{
        display: none;
    }
  

    .header-phone li{
        list-style: none;
        background: white;
        border: 1px solid rgb(241, 241, 241);
        color: black;
        font-size: 25px;
        padding: 10px 0 10px 25px;

        cursor: pointer;
        text-align: left;
    }

     .header-phone li:hover{
        background: #171772ad;
        color: white;
        transition: .5s;
     }


    a:visited{
        color: inherit;
    }
     a{
        text-decoration: none;
    }

.close {
    display: none;
}

.close-active {
    display: block;
    height: 30px;
}

}
</style>