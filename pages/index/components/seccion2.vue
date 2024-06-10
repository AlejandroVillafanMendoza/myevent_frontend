<template>

        <div class="H1">¡¡descubre lo que tenemos para ti!!</div>
                <button class="Boton" @click="nuestras_ofertas">
                    <img src="/public/img/productos_boton.png" alt="">
                </button>

        <div class="H1">¡¡Lo que tenemo para TI!!</div>
                <v-container>
                    <div>
                <button class="Boton_2" @click="gotokids">
                <img src="/public/img/kids_boton.png" alt="">
                </button>
                <button class="Boton_2" @click="gotopremium">
                <img src="/public/img/premium_boton.png" alt="">
                </button>
                <button class="Boton_2" @click="gotowedding">
                <img src="/public/img/weddig_boton.png" alt="">
                </button>
                <button class="Boton_2" @click="gotoxv" >
                <img src="/public/img/xv_boton.png" alt="">
                </button>
                    </div>
                </v-container>
               
                
</template>

<script setup>
  const nuestras_ofertas = () => {
      window.location.href = '/products'; 
    }
  const gotokids =() => {
    window.location.href = '/kids'
  }
   const gotopremium = () => {
    window.location.href = '/premium'
   }
   const gotoxv = () => {
    window.location.href = '/party'
   }
   const gotowedding = () => {
    window.location.href = '/wedding'
   }
</script>

<style>

.H1{
    text-align: center;
    text-transform: uppercase;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 30px;
    font-weight: 700;
    color:#73f0eb; 
}
.Boton{
    width: auto;
    height: auto;
    border-radius: 12px;
    padding: 10px 545px;
    cursor: pointer;
        }

.Boton img{
    display: block;
    width: auto;  
    height: auto;  
    border-radius: 12px;
}
.Boton img:hover{
    transform: scale(1.5);

}

.Boton_2{

    width: auto;
    height: auto;
    border-radius: 12px;
    margin-left: 95px;
    margin-top: 50px;
    cursor: pointer;
}
.Boton_2 img{
border-radius: 12px;

}

.Boton_2:hover{
    transform: scale(1.2);
}
</style>