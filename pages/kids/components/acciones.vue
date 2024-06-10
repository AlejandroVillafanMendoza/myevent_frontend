<template>
    
    <v-container class="cont">
        <v-btn class="action" @click="gotostar">Volver al inicio</v-btn>
        <v-btn class="action" @click="gotoorg">Organizar tu evento</v-btn>
        <v-btn class="action" @click="gotopro">Producto y Servicios</v-btn>
        
    </v-container>
</template>

<script setup>
const gotostar = () => {
    window.location.href = '/'
}
const gotoorg = () => {
    window.location.href = '/organiza'
}
const gotopro = () => {
    window.location.href = '/products'

}
</script>

<style>
.action{
   text-align: center;
   width: auto;
   background-color: #ffc0cb;
   color: #ffff;
   margin-left: 79px;
   margin-right: 100px;
   
   

}

</style>