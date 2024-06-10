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
    { titulo: ' Fiesta para niños', subtitulo: 'De 0-5 años', text: 'Haz que tu niños tengan un experiencia inovidable', image: '/img/kids_3.jpg' },
    { titulo: 'Cenas de Gala', subtitulo: 'Ejecutiva', text: 'Brinda a tu equipo, una noche de divercion', image: '/img/premium_1.jpg' },
    { titulo: 'Titulo 3', subtitulo: 'Subtitulo 3', text: 'Texto 3', image: 'https://cdn.vuetifyjs.com/images/cards/road.jpg' },
    // Agrega más objetos aquí si es necesario
  ]
  </script>
  

