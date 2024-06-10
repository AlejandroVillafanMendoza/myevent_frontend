<template>
  <v-carousel height="600px">
    <v-carousel-item
      v-for="(item, index) in items" :key="index"
      :src="item.image"
      cover
    >
      <div class="carousel-caption">
        <h3 class="titulo">{{ item.title }}</h3>
        <p class="des">{{ item.description }}</p>
     <!--   <v-btn class="ira">Ir a</v-btn> -->
      </div>
    </v-carousel-item>
  </v-carousel>

</template>
<script setup>
import { ref } from 'vue';

const items = ref([
  {
    image: 'img/wedding_carrusel.png',
    title: "BODAS",
    description: "Hecha un vistazo a todo lo que tenemos para tu boda",
  },
  {
    image: 'img/xv_carrusel.png',
    title: "XV AÑÓS",
    description: "Hecha un vistazo a lo que tenemos para tus XV Años"
  },
  {
    image:'img/kids_carrusel.png',
    title: "KIDS",
    description:"Hecha un vistazo a lo que tenemos para los consentidos del hogar"
  },  
    {
      image:'img/premium_carrucel.png',
      title: "PREMIUM",
      description:"Hecha un vistazo a lo que tenemos para tus reuniones de Gala"     
    },
]);
</script>

<style scoped>

.carousel-caption {
  position: absolute;
  bottom: 55px;
  left: 50%;
  transform: translateX(-50%);
  color: rgb(255, 255, 255);
  background-color:#000000ae;
  padding: 10px;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  width: 250px;
  height: auto;
}
.titulo{
  text-align: center;
  text-transform: uppercase;
  color:#ffff;
}

.ira{
    color: #42d6d6;
    border-bottom-color: black;
    border: 10px;
    text-align: center;
    font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
    font-size: larger;
    margin-top: 5px;
    margin-bottom: 2px;
}

</style>
  