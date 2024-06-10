
<template>
    <v-container>
      <v-row>
        <v-col
          v-for="(item, index) in items"
          :key="index"
          cols="12"
          md="4"
        >
          <v-card class="mx-auto" max-width="400">
            <v-img :src="item.image" height="200px" cover></v-img>
            <v-card-title>{{ item.titulo }}</v-card-title>
            <v-card-subtitle>{{ item.subtitulo }}</v-card-subtitle>
            <v-card-text>{{ item.text }}</v-card-text>
            <v-card-actions>
              <v-btn color="orange-lighten-2" text>Explore</v-btn>
              <v-spacer></v-spacer>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </template>
  
  <script setup>
  const items = [
    { titulo: 'Cena de Gala', 
    subtitulo: 'Desde 1.500 $', 
    text: 'Organiza tu cena de gala para compartir un momento especial', 
    image: '/img/premium_cards/premium_card_1.jpg' },

    { titulo: 'Cena de Año Nuevo', 
    subtitulo: 'Desde 2.500 $', 
    text: 'Que tu nuevo año empieze de la mejor cena del año', 
    image: '/img/premium_cards/premium_card_2.jpg' },

    { titulo: 'Cena Naideña', 
    subtitulo: 'Desde 2.500 $', 
    text: 'Que el Espiritu Navideño corra por toda la noche con tu increible fiesta', 
    image: '/img/premium_cards/premium_card_3.jpg' },

    { titulo: 'Entrega de Premios', 
    subtitulo: 'Desde 2.500$', 
    text: 'Celebra tus logros con un evento a la altura', 
    image: '/img/premium_cards/premium_card_4.jpg' },

    { titulo: 'Fiesta de Graduacion', 
    subtitulo: 'Desde 2.500$', 
    text: 'Cierra tu año escolar de la mejor manera ', 
    image: '/img/premium_cards/premium_card_5.jpg' },

    { titulo: 'Fiesta Ejecutiva', 
    subtitulo: 'Desde 2.500$', 
    text: 'Celebra con tus compañeros de trabajo', 
    image: '/img/premium_cards/premium_card_6.jpg' },

 
  ]
  </script>
  
  