
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
  { titulo: 'Vestidos de Novia ', 
    subtitulo: 'Desde 1.500$', 
    text: '', 
    image: '/img/wedding_cards/wedding_card_1.jpg' },

    { titulo: 'Traje de novio', 
    subtitulo: 'Desde 1.500$', 
    text: '', 
    image: '/img/wedding_cards/wedding_card_2.jpg' },

    { titulo: 'Ramos de novia', 
    subtitulo: 'Desde 25$', 
    text: '', 
    image: '/img/wedding_cards/wedding_card_3.jpg' },

    { titulo: 'Pateles de Boda', 
    subtitulo: 'Desde 2.000$', 
    text: '', 
    image: '/img/wedding_cards/wedding_card_4.jpg' },

    { titulo: 'Centros de Mesa', 
    subtitulo: 'Desde 50$ 12 unidades', 
    text: '', 
    image: '/img/wedding_cards/wedding_card_5.jpg' },

    { titulo: 'Decoraciones', 
    subtitulo: 'Desde 1.500$', 
    text: '', 
    image: '/img/wedding_cards/wedding_card_6.jpg' },
  ]
  </script>
  
  