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
        </div>
      </v-carousel-item>
    </v-carousel>
  
  </template>
  <script setup>
  import { ref } from 'vue';
  
  const items = ref([
    {
      image: 'img/xv_carrusel.png',
      title: "",
      description: "Haz que tus niños tengan una experiencia inolvidable",
    },
    {
      image: 'img/xv_1.jpg',
      title: "",
      description: "Hecha un vistazo a lo que tenemos para tus XV Años"
    },
    {
      image:'img/xv_2.jpg',
      title: "",
      description:"Hecha un vistazo a lo que tenemos para los consentidos del hogar"
    },  
      {
        image:'img/xv_3.jpg',
        title: "",
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
  
  </style>
    