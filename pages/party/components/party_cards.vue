
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
    { titulo: 'Decoracion', 
    subtitulo: 'Desde 1.500$', 
    text: '', 
    image: '/img/xv_cards/xv_card_1.jpg' },


    { titulo: 'Vestidos para XV', 
    subtitulo: 'Desde 2.500$', 
    text: '', 
    image: '/img/xv_cards/xv_card_2.jpg' },
    
    { titulo: 'Centros de Mesa', 
    subtitulo: 'desde 50$ c/u', 
    text: '', 
    image: '/img/xv_cards/xv_card_3.jpg' },

    { titulo: 'Pateles para XV', 
    subtitulo: 'Desde 1.500$', 
    text: '', 
    image: '/img/xv_cards/xv_card_4.jpg' },

    { titulo: 'Recuerditos', 
    subtitulo: '5$ C/U', 
    text: '', 
    image: '/img/xv_cards/xv_card_5.jpg' },

    { titulo: 'Tiaras', 
    subtitulo: '15$', 
    text: 'Texto 1', 
    image: '/img/xv_cards/xv_card_6.jpg' },

  ]
  </script>
  
  